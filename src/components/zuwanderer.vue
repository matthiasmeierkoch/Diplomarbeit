<template>
    <div class="map2">
        <h3 class="map__title">{{title}}:</h3>
        <div style="position:relative;">
            <div id="map2"/>
            <div class="legend">
            <div v-for="threshold in thresholds" style="display:flex;margin-bottom:0.25rem;align-items:center;">
                <div v-bind:style="{ background: threshold.color, width: '1.5rem', height: '1.5rem', marginRight: '0.75rem' }"/>
                <div style="font-family:'Suisse BP Int';font-size:0.875rem;">
                    {{ threshold.step }}
                </div>
            </div>
        </div>
    </div>
    <p>Quelle der Daten:
        <a href="https://opendata.swiss/de/dataset/umzuge-nach-stadtquartier-geschlecht-altersgruppe-und-zivilstand-seit-19931/resource/27051ba4-ccf1-43de-8d4e-a97ea1c37959">
            opendata.swiss</a></p>
    </div>
</template>

<script>

    import {json, csv} from "d3-fetch"
    import {feature} from "topojson-client"
    import {geoPath, geoAzimuthalEqualArea} from "d3-geo"
    import {select} from "d3-selection"
    import {scaleLinear, scaleQuantize} from "d3-scale"
    import {extent} from "d3-array"

    const width = 400
    const height = 400

    export default {
        data: function () {
            return {
                message: "Hello, world!",
                thresholds: [],
            }
        },
        methods: {
            parseGeographies(d) {
                return feature(d, d.objects.stadtkreise).features
            },
            getProjection(w, h) {
                return geoAzimuthalEqualArea()
                    .translate([w / 2, h / 2])
                    .rotate([-8.5417, -47.3769, 0])
                    .center([-0.01, -0.005])
                    .scale(150000)
            },
            getGeographyData() {
                return json("/stadt-zurich.json")
            },
            getDistrictsData() {
                return csv("/Zuwanderer.csv")
            },
        },
        async mounted() {
            console.log("Hello")
            Promise.all([
                this.getGeographyData(),
                this.getDistrictsData(),
            ]).then(([geoData, csvData]) => {
                const features = this.parseGeographies(geoData)
                const districtData = csvData
                console.log(csvData)
                const svg = select("#map2")
                    .append("svg")
                    .attr("viewBox", `0 0 ${width} ${height}`)

                const projection = this.getProjection(width, height)
                const path = geoPath().projection(projection)

                const ext = extent(districtData, d => +d.Zuwanderer)

                const colors = ["#c4dcff", "#a7bfe5", "#8ba3c7", "#6f88ab", "#556e90", "#3b5575", "#213d5c", "#032743",]

                const scale = scaleQuantize()
                    .domain([0, ext[1]])
                    .range(colors)
                    .nice()

                const steps = [
                    scale.domain()[0],
                    ...scale.thresholds(),
                    scale.domain()[1],
                ]

                this.thresholds = steps.map((d, i) => {
                    return {step: `${d} - ${steps[i + 1]}`, color: colors[i]}
                }).slice(0, -1).reverse()

                const kreise = svg.selectAll("path")
                    .data(features)
                    .enter()
                    .append("path")
                    .attr("d", path)
                    .attr("fill", d => {
                        const relevantData = districtData.find(s => s.KNr === d.id)
                        return scale(relevantData.Zuwanderer)
                    })
                    .attr("stroke", "#FFF")
                    .attr("stroke-width", 0.7)
                    .on("click", d => {
                        const relevantData = districtData.find(s => s.KNr === d.id)
                    })

                const labels = svg.selectAll("text")
                    .data(features)
                    .enter()
                    .append("text")
                    .attr("x", d => {
                        return path.centroid(d)[0]
                    })
                    .attr("y", d => {
                        return path.centroid(d)[1]
                    })
                    .attr("textAnchor", "middle")
                    .attr("alignment-baseline", "middle")
                    .attr("font-size", "0.5rem")
                    .attr("fill", "#FFF")
                    /*
                                        .text(d => d.id)
                    */
                    .text(d => {
                        const relevantData = districtData.find(s => s.KNr === d.id)
                        return relevantData.Zuwanderer
                    })
            })

        },
        props: ['title']
    }
</script>

<style>

    .legend{
        position: absolute;
        bottom: 2.5rem;
        left: 2.5rem;
    }

    .map2 {
        background-color: #FCFBF9;
        padding-top: 2rem;
        padding-left: 4rem;
        padding-right: 4rem;
        padding-bottom: 2rem;
        max-width: 100%;
        margin-top: 4rem;
        margin-bottom: 2rem;
        margin-left: auto;
        margin-right: auto;
        border-radius: 24px;
    }

    #map2 {
        margin-top: -1.5rem;
    }

    .map__title {
        color: #003041;
    }

    @media (max-width: 667px) {
        .legend {
            position: relative;

        }

        #map2 {
            margin-top: auto;
        }
    }

</style>
