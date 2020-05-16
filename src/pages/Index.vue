<template>
    <Layout>
        <!-- Learn how to use images here: https://gridsome.org/docs/images -->
        <h1 class="item-a">Willkommen in Wiedikon</h1>
        <div class="container">

        <lead>
            <p> Jedes Jahr ziehen zwischen 41000 und 46000 Personen nach Zürich und der grösste
                Teil der Zuwanderer sind Ausländer. Im Jahr 2017 sind ca. 3500 Zürcher nach Wiedikon gezogen.
                Für viele ist ein Umzug und besonders ein Kantons oder sogar Landeswechsel immer auch mit Komplikationen
                und Unsicherheiten verbunden.
            </p>
        </lead>

            <chapter title="Einleitung">
            <p> Wie verhält man sich richtig? wie integriere ich mich möglichst schnell und einfach in ein bestehendes Quartierleben?
                und wo finde ich Antworten auf Fragen wie diese?
            </p>
            </chapter>

            <g-image src="../assets/img/zurich.jpg" height="800" fit="cover"/>

            <chapter title="Auswertung der Umfrage">
            <p> In einem Vorprojekt habe ich eine Umfrage mit bewohner der Kreis 3 durchgeführt, in dieser ich auf das
                Verhalten und dernen Bedür-fnisse eingegangen bin.
                Mithilfe dieser Einblicke habe ich eine Zielgruppe und Bedürfnissanalyse Zusammengestellt welche hier
                heruntergeladen werden kann.
                <br>
                <a href="../assets/uploads/wiso-so-neugierig.pdf">Auswertung des Vorprojekt als PDF
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><title>
                        download_icon</title>
                        <g class="nc-icon-wrapper" fill="#0070BC">
                            <path d="M19 9h-4V3H9v6H5l7 7 7-7zM5 18v2h14v-2H5z"/>
                        </g>
                    </svg>
                </a>

            </p>
        </chapter>

        <chapter title="User Journey">
            <p> In einem Vorprojekt habe ich eine Umfrage mit bewohner der Kreis 3 durchgeführt, in dieser ich auf das
                Verhalten und dernen Bedür-fnisse eingegangen bin.
                Mithilfe dieser Einblicke habe ich eine Zielgruppe und Bedürfnissanalyse Zusammengestellt welche hier
                heruntergeladen werden kann.
                <br>
            </p>
        </chapter>

        <chapter title="Benutzerrollen">
            <p> In einem Vorprojekt habe ich eine Umfrage mit bewohner der Kreis 3 durchgeführt, in dieser ich auf das
                Verhalten und dernen Bedür-fnisse eingegangen bin.
                Mithilfe dieser Einblicke habe ich eine Zielgruppe und Bedürfnissanalyse Zusammengestellt welche hier
                heruntergeladen werden kann.
                <br>
            </p>
        </chapter>

        <chapter title="Personas">
            <p> In einem Vorprojekt habe ich eine Umfrage mit bewohner der Kreis 3 durchgeführt, in dieser ich auf das
                Verhalten und dernen Bedür-fnisse eingegangen bin.
                Mithilfe dieser Einblicke habe ich eine Zielgruppe und Bedürfnissanalyse Zusammengestellt welche hier
                heruntergeladen werden kann.
                <br>

            </p>
        </chapter>

        <chapter title="Konzept">
            <p> In einem Vorprojekt habe ich eine Umfrage mit bewohner der Kreis 3 durchgeführt, in dieser ich auf das
                Verhalten und dernen Bedür-fnisse eingegangen bin.
                Mithilfe dieser Einblicke habe ich eine Zielgruppe und Bedürfnissanalyse Zusammengestellt welche hier
                heruntergeladen werden kann.
                <br>
            </p>
        </chapter>

        <p class="home-links">
            <a href="https://gridsome.org/docs/" target="_blank" rel="noopener">Gridsome Docs</a>
            <a href="https://github.com/gridsome/gridsome" target="_blank" rel="noopener">GitHub</a>
        </p>
        </div>
    </Layout>
</template>

<script>
    import Chapter from "../components/chapter"
    import Lead from "../components/lead"

    export default {
        metaInfo: {
            title: 'Willkommen in Wiedikon'
        },
        components: {
            Chapter,
            Lead
        }
    }
</script>

<style>
    @import url('https://rsms.me/inter/inter.css');

    .container {

    }

    svg {
        padding-top: 0.5rem;
    }

    img{
        width:100%;
        fit: cover;

    }

    p a {
        color: #0070BC;
        text-decoration: none;
    }

    p a:hover {
        color: #0070BC;
        text-decoration: underline;
    }

    .home-links a {
        margin-top: 3rem;
        margin-right: 1rem;
        color: #0070BC;

    }

    h1 {
        font-size: 5.125rem;
        line-height: 5.125rem;
        color: #0070BC;
        width: 30rem;
    }

    @media (max-width: 667px) {

        h1 {
            font-size: 4.25rem;
            width: 100%;
            line-height: 4.25rem;
        }
    }


</style>
