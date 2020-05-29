<template>
    <Layout>
        <!-- Learn how to use images here: https://gridsome.org/docs/images -->
        <div class="container">
            <welcome/>

            <lead>
                <p> In den letzten Jahren sind zwischen 41&#x202F;000 und 46&#x202F;000 Personen nach Zürich gezogen.
                    Für viele ist
                    ein Umzug und besonders ein Kantons oder sogar Landeswechsel immer auch mit Komplikationen und
                    Unsicherheiten verbunden.
                </p>
            </lead>


            <chapter title="Einleitung">
                <p> Wie integriere ich mich möglichst schnell und einfach in das bestehendes Quartierleben des Kreis 3?
                    Wie kann ich den Kreis 3 besser kennenlernen und wo finde ich Antworten auf meine Fragen zu meinem
                    Kreis?
                </p>
                <p>
                    Mit diesen Problemen habe ich mich in meiner Diplomarbeit auseinandergesetzt. Dafür habe ich eine
                    App konzipiert und gestaltet welche neuen und bestehenden Bewohner des Kreis 3 eine neue Möglichkeit
                    gibt Ihr Kreis zu entdecken und sich in der Community mit einzubringen.
                </p>
                <p>
                    Der Kreis 3 umfasst die Quartiere: Sihlfeld, Alt-Wiedikon und Friesenberg. 2019 lebten 51 122
                    Personen im Kreis 3, damit ist es der am zweit stärksten bevölkerte Kreis in Zürich.
                </p>
            </chapter>

            <div>
                <Population title="Bevölkerung Stadt Zürich 2019"></Population>
            </div>

            <div>
                <Zuwanderer title="Zuwanderer aus einem anderen Kreis 2019"></Zuwanderer>
            </div>


            <chapter title="Research & Befragung der Zielgruppe:">
                <p> Besonders weil ich einen persönlichen Bezug zu diesem Thema habe, da ich selber neu in den Kreis 3
                    gezogen bin war es mir wichtig in meiner Erarbeitung objektive Entscheidungen zu treffen und diese
                    wenn immer möglich auf Daten zu stützen. Daher und um mich vertieft mit meiner Fragestellungen
                    auseinander zusetzten habe ich mich als ersten Schritt mit den betroffenen direkt ausgetauscht und
                    habe 17 Zuzügler und Zuzüglerinnen von Wiedikon befragt.
                </p>
                <p>
                    In meiner Befragung habe ich darauf abgezielt zu verstehen welche Bedürfnisse neue Bewohner im Kreis
                    3 haben. Zuwanderer die schon länger im Quartier wohnen habe ich über ihr Informationsverhalten, ihr
                    Engagement im Kreis, Tips und Tricks die ihnen geholfen haben als Sie neu im Quartier ware befragt.
                </p>
                <Quote title="Zitat aus der Befragung">
                    <p>«Profitiert habe ich vor allem von Personen die schon länger hier wohnen und Bescheid wissen was
                        wo läuft»</p>
                </Quote>
                <p>
                    Die Befragungen haben gezeigt dass die meisten Zuwanderer besonders von Tips und Empfehlungen von
                    Freuenden und einem bestehenden Umfeld profitieren konnten. Nach den persönlichen Empfehlungen ist
                    bei meinen Befragungen Facebook auf dem zweiten Platz. Da jüngeren vermehrt auf Facebook verzichten,
                    könnten Sie besonders auf die Empfehlungen anderer angewiesen sein.
                </p>
                <p>
                    Komplette Auswertung der Daten CSV:
                    <a class="home-links" href="../assets/uploads/Zürcher%20Zuwanderer%20Umfrage.csv"> Download
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 -5 24 24"><title>
                            download_icon</title>
                            <g class="nc-icon-wrapper" fill="#E4665C">
                                <path d="M19 9h-4V3H9v6H5l7 7 7-7zM5 18v2h14v-2H5z"/>
                            </g>
                        </svg>
                    </a>
                </p>
            </chapter>

            <chapter title="Markt- und Konkurrenzanalyse»">
                <p> Gibt es bereits Applikationen die meine Problemstellung lösen? Oder zumindest Teilweise abdecken?
                    Ich habe mir folgende Angebote genauer angesehen:
                </p>
                <p>
                    «Hello Zürich» Das Stadtmagazin punktet mit seinen besonders gut aufbereiteten redaktionellen
                    Artikel und den Möglichkeiten seine Lieblingsorte zu speichern. Leider kommt dafür der Austausch in
                    einer Community und das Profitieren von anderen Erfahrungen zu kurz.
                </p>
                <p>
                    «AirBnb» AirBnb gehört mit seinem breiten Angebo und den Entdeckungsmöglichkeiten ebenfalls zu einer
                    art Konkurrenz, auch hier fehlt leider der Community teil.
                </p>
                <p>
                    Wer also pflegt eine Community?
                    Ich habe mir dazu Applikationen der Bauindustrie angesehen, in den letzten Jahren sind bei grösseren
                    Überbauungen vermehrt Applikationen eingesetzt worden welche die Community innerhalb der Überbauung
                    fördern soll, bei diesen Applikationen steht jedoch oft auch die Wohnung eines Mieter im
                    Vordergrund.
                </p>
            </chapter>

            <chapter title="Ideation">
                <p> In einem Vorprojekt habe ich eine Umfrage mit bewohner der Kreis 3 durchgeführt, in dieser ich auf
                    das
                    Verhalten und dernen Bedür-fnisse eingegangen bin.
                    Mithilfe dieser Einblicke habe ich eine Zielgruppe und Bedürfnissanalyse Zusammengestellt welche
                    hier
                    heruntergeladen werden kann. </p>
                <br>
                <Quote title="Linus Pauling">
                    <p>«Der einfachste Weg zu einer guten Idee, ist viele Ideen zu haben.»</p>
                </Quote>
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
            <Weekday/>
        </div>
        <Background/>
    </Layout>
</template>

<script>

    import welcome from "../components/welcome"
    import Chapter from "../components/chapter"
    import Lead from "../components/lead"
    import Weekday from "../components/weekday"
    import Background from "../components/background.vue"
    import Quote from "../components/Quote.vue"
    import Population from "../components/population.vue";
    import Zuwanderer from "../components/zuwanderer.vue";
    import sal from "sal.js";

    export default {
        metaInfo: {
            title: 'Willkommen im Kreis 3 in Zürich'
        },
        components: {
            Zuwanderer,
            Population,
            welcome,
            Chapter,
            Lead,
            Weekday,
            Background,
            Quote
        },

        mounted() {
            this.$nextTick(() => sal());
        }
    }
</script>

<style>
    html{
        overflow-x:hidden;
    }


    .container {
        max-width: 75ch;
        margin: auto;
        z-index: 10;
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
