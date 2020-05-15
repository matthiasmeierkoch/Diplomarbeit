<template>
    <Layout>
        <!-- Learn how to use images here: https://gridsome.org/docs/images -->
        <h1 class="item-a">Willkommen in Wiedikon</h1>
        <div class="container"
        <chapter title="Herleitung">
            <p> Zwischen 2006 und 2016 sind zwischen 41000 und 46000 Personen im Jahr nach Zürich gezogen. Der grösste
                Teil der Zuwanderer sind Ausländer.
                Für viele ist ein Kantonswechsel und besonders ein Landeswechsel mit komplikationen und Unsicherheiten
                verbunden. Wie verhält man sich richtig? und was ist hier anders als gewohnt? Und wo finde ich die
                Antworten auf diese Fragen?
                Zudem möchte man sich möglichst schnell einleben und im neuen Zuhause einleben und in der Gesellschaft
                integrienen. </p>
        </chapter>

        <chapter title="Vorprojekt">
            <p> In einem Vorprojekt habe ich eine Umfrage mit bewohner der Kreis 3 durchgeführt, in dieser ich auf das
                Verhalten und dernen Bedür-fnisse eingegangen bin.
                Mithilfe dieser Einblicke habe ich eine Zielgruppe und Bedürfnissanalyse Zusammengestellt welche hier
                heruntergeladen werden kann.
                <br>
                <a href="../assets/uploads/html5-css-referenz.pdf">Auswertung des Vorprojekt als PDF
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><title>
                        download_icon</title>
                        <g class="nc-icon-wrapper" fill="#ED8A53">
                            <path d="M19 9h-4V3H9v6H5l7 7 7-7zM5 18v2h14v-2H5z"/>
                        </g>
                    </svg>
                </a>

            </p>
        </chapter>

        <p class="home-links">
            <a href="https://gridsome.org/docs/" target="_blank" rel="noopener">Gridsome Docs</a>
            <a href="https://github.com/gridsome/gridsome" target="_blank" rel="noopener">GitHub</a>
        </p>

    </Layout>
</template>

<script>
    import Chapter from "../components/chapter"

    export default {
        metaInfo: {
            title: 'Willkommen in Wiedikon'
        },
        components: {
            Chapter
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

    p a {
        color: #ED8A53;
        text-decoration: none;
    }

    p a:hover {
        color: #ED8A53;
        text-decoration: underline;
    }

    .home-links a {
        margin-right: 1rem;
        font-family: Inter;
        color: #ED8A53;

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
