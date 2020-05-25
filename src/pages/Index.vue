<template>
    <Layout>
        <vue-read-progress></vue-read-progress>
        <!-- Learn how to use images here: https://gridsome.org/docs/images -->
        <div class="container">
            <welcome/>

            <lead>
                <p> In den letzten Jahren sind zwischen 41&#x202F;000 und 46&#x202F;000 Personen nach Zürich gezogen,
                    davon sind rund 24&#x202F;334 Personen in die Stadt Zürich gezogen.
                    Der Kreis 3 hat dadurch in den Letzten Jahren einen zuwachs von rund
                    Im Jahr 2017 sind ca. 3500 Zürcher nach Wiedikon gezogen.
                    Für viele ist ein Umzug und besonders ein Kantons oder sogar Landeswechsel immer auch mit
                    Komplikationen
                    und Unsicherheiten verbunden.
                </p>
            </lead>

            <Map/>

            <chapter title="Einleitung">
                <p> Wie integriere ich mich möglichst schnell und einfach in ein
                    bestehendes Quartierleben? Wie kann ich mein Quartier besser kennenlernen und wo finde ich Antworten
                    auf Fragen zum Quartierleben?
                <p> Mit diesen Fragestellungen habe ich mich in meiner Diplomarbeit auseinandergesetzt.</p>
                </p>
            </chapter>

        </div>
        <!--<g-image src="../assets/img/zurich.jpg" height="800" fit="cover"/>-->
        <div class="container">
            <chapter title="Befragung der Zielgruppe:">
                <p> Um mich vertieft mit meiner Fragestellungen auseinander zusetzten habe ich als ersten schritt den
                    betroffenen direkt ausgetauscht und habe 17 Zuzügler und Zuzüglerinnen nach Wiedikon befragt.
                </p>
                <p>
                    In meiner Befragung habe ich besonders darauf abgezielt zu verstehen welche Probleme dass neue in
                    einem Quartier haben. Zuwanderer die schon länger im Quartier wohnen habe ich über ihr
                    informationsverhalten, ihr Engagement im Quartier, Tips und Tricks die ihnen geholfen haben als Sie
                    neu im Quartier ware ect.
                </p>
                <Quote title="Zitat aus der Befragung">
                    <p>«Profitiert habe ich vor allem von Personen die schon länger hier wohnen und Bescheid wissen was wo läuft»</p>
                </Quote>
                <p>
                    Die Befragungen haben gezeigt dass die meisten Zuwanderer besonders von Tips und Empfehlungen von
                    Freuenden und einem bestehenden Umfeld profitieren konnten. Nach dem persönlichen Empfehlungen ist
                    bei meinen Befragungen Facebook auf dem zweiten Platz. Da jüngeren vermehrt auf Facebook verzichten,
                    könnten Sie besonders auf ander Empfehlungen angewiesen sein.
                </p>
                <p>
                    Komplette Auswertung der Daten CSV:
                    <a class="home-links" href="../assets/uploads/wiso-so-neugierig.pdf"> Download
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 -5 24 24"><title>
                            download_icon</title>
                            <g class="nc-icon-wrapper" fill="#E4665C">
                                <path d="M19 9h-4V3H9v6H5l7 7 7-7zM5 18v2h14v-2H5z"/>
                            </g>
                        </svg>
                    </a>
                </p>
            </chapter>

            <chapter title="Ideation">
                <p> In einem Vorprojekt habe ich eine Umfrage mit bewohner der Kreis 3 durchgeführt, in dieser ich auf
                    das
                    Verhalten und dernen Bedür-fnisse eingegangen bin.
                    Mithilfe dieser Einblicke habe ich eine Zielgruppe und Bedürfnissanalyse Zusammengestellt welche
                    hier
                    heruntergeladen werden kann.
                    <br>
                </p>
            </chapter>

            <chapter title="Benutzerrollen">
                <p> In einem Vorprojekt habe ich eine Umfrage mit bewohner der Kreis 3 durchgeführt, in dieser ich auf
                    das
                    Verhalten und dernen Bedür-fnisse eingegangen bin.
                    Mithilfe dieser Einblicke habe ich eine Zielgruppe und Bedürfnissanalyse Zusammengestellt welche
                    hier
                    heruntergeladen werden kann.
                    <br>
                </p>
            </chapter>


            <p class="home-links">
                <Weekday/>
                <a href="https://gridsome.org/docs/" target="_blank" rel="noopener">Gridsome Docs</a>
                <a href="https://github.com/gridsome/gridsome" target="_blank" rel="noopener">GitHub</a>
            </p>
        </div>

        <Background/>
    </Layout>
</template>

<script>
    import * as d3 from 'd3'

    import welcome from "../components/welcome"
    import Chapter from "../components/chapter"
    import Lead from "../components/lead"
    import Weekday from "../components/weekday"
    import Map from "../components/map.vue"
    import Background from "../components/background.vue"
    import Quote from "../components/Quote.vue"
    import VueReadProgress from "vue-read-progress";


    export default {
        metaInfo: {
            title: 'Willkommen im Kreis 3 in Zürich'
        },
        components: {
            welcome,
            Chapter,
            Lead,
            Map,
            Weekday,
            Background,
            VueReadProgress,
            Quote
        }
    }
</script>

<style>

    .container {
        max-width: 75ch;
        margin: auto;
    }

    svg {
        padding-top: 0.5rem;
    }


    img {
        width: 100%;
    }

    p a {
        color: #E4665C;
        text-decoration: none;
    }

    p a:hover {
        color: #111111;
        fill: #111111;
        text-decoration: underline;
    }

    .home-links a {
        margin-top: 3rem;
        margin-right: 1rem;
        color: #E4665C;
    }

</style>
