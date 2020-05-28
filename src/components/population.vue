<template>
    <div class="map1">
        <h3 class="map__title">{{title}}:</h3>
        <div style="position:relative;">
            <div id="map1" />
            <div class="legend" style="position:absolute;bottom:2.5rem;left:2.5rem;">
                <div v-for="threshold in thresholds" style="display:flex;margin-bottom:0.25rem;align-items:center;">
                    <div v-bind:style="{ background: threshold.color, width: '1.5rem', height: '1.5rem', marginRight: '0.75rem' }" />
                    <div style="font-family:'Suisse BP Int';font-size:0.875rem;">
                        {{ threshold.step }}
                    </div>
                </div>
            </div>
        </div>
        <p>Quelle der Daten:
            <a href="https://data.stadt-zuerich.ch/dataset/bev_bestand_jahr_quartier_nationalitaet_od3361">
                Open Data Zürich</a></p>
    </div>
</template>

<script>

    import { json, csv } from "d3-fetch"
    import { feature } from "topojson-client"
    import { geoPath, geoAzimuthalEqualArea } from "d3-geo"
    import { select } from "d3-selection"
    import { scaleLinear, scaleQuantize } from "d3-scale"
    import { extent } from "d3-array"

    const width = 400
    const height = 400

    export default {
        data: function() {
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
                return json("https://statistikstadtzuerich.github.io/sszvis/topo/stadt-zurich.json")
            },
            getDistrictsData() {
                return csv("https://statistikstadtzuerich.github.io/sszvis/map-standard/data/M_kreis.csv")
            },
        },
        async mounted() {

            Promise.all([
                this.getGeographyData(),
                this.getDistrictsData(),
            ]).then(([ geoData, csvData ]) => {
                const features = this.parseGeographies(geoData)
                const districtData = csvData

                const svg = select("#map1")
                    .append("svg")
                    .attr("viewBox", `0 0 ${width} ${height}`)

                const projection = this.getProjection(width, height)
                const path = geoPath().projection(projection)

                const ext = extent(districtData, d => +d.Bevölkerung)

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
                    return { step: `${d} - ${steps[i+1]}`, color: colors[i] }
                }).slice(0, -1).reverse()

                const kreise = svg.selectAll("path")
                    .data(features)
                    .enter()
                    .append("path")
                    .attr("d", path)
                    .attr("fill", d => {
                        const relevantData = districtData.find(s => s.KNr === d.id)
                        return scale(relevantData.Bevölkerung)
                    })
                    .attr("stroke", "#FFF")
                    .attr("stroke-width", 0.7)
                    .on("click", d => {
                        const relevantData = districtData.find(s => s.KNr === d.id)
                        console.log(relevantData)
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
                    .text(d => {
                        const relevantData = districtData.find(s => s.KNr === d.id)
                        return relevantData.Bevölkerung
                    })
            })

        },
        props: ['title']
    }
</script>

<style>
    .map1{
        background-color: #FCFBF9;
        padding-top:2rem;
        padding-left:4rem;
        padding-right:4rem;
        padding-bottom:2rem;
        max-width: 100%;
        margin-top: 2rem;
        margin-bottom: 2rem;
        margin-left: auto;
        margin-right: auto;
        border-radius: 24px;
    }

    #map1{
        margin-top: -1.5rem;
    }
.map__title{
    color: #003041;
}

    @media (max-width: 667px) {
        .legend{
            position: relative;
        }

        #map1{
            margin-top: auto;
        }
    }

</style>