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
                <p> Wie integriere ich mich möglichst schnell und einfach in das bestehendes Quartierleben des Kreis 3
                    integrieren? Und wie kann ich den Kreis 3 besser kennenlernen?
                </p>
                <p>
                    Mit diesen Problemen habe ich mich in meiner Diplomarbeit auseinandergesetzt. Dafür habe ich eine
                    App konzipiert und gestaltet welche neuen und bestehenden Bewohner des Kreis 3 eine neue Möglichkeit
                    gibt Ihr Kreis zu entdecken und sich in der Community mit einzubringen.
                </p>
                <p>
                    Der Kreis 3 umfasst die Quartiere: Sihlfeld, Alt-Wiedikon und Friesenberg. 2019 lebten etwas über 45&#x202F;000
                    Personen im Kreis 3, damit ist er der am zweit stärksten bevölkerte Kreis in Zürich.
                </p>
            </chapter>

            <div>
                <Population data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
                            data-sal-easing="ease-out-bounce" title="Bevölkerung Stadt Zürich 2019"></Population>
            </div>
            <p>
                Im Jahr 2019 war es der Kreis der am dritt meisten Zuzügler von anderen Kreisen der Stadt Zürich
                verzeichnete.
            </p>

            <div>
                <Zuwanderer data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
                            data-sal-easing="ease-out-bounce"
                            title="Zuwanderer aus einem anderen Kreis 2019"></Zuwanderer>
            </div>

            <chapter title="Befragung der Zielgruppe:">
                <p> Besonders weil ich einen persönlichen Bezug zu diesem Thema habe, da ich selber neu in den Kreis 3
                    gezogen bin war es mir wichtig in meiner Erarbeitung objektive Entscheidungen zu treffen und diese
                    wenn immer möglich auf Daten zu stützen. Daher und um mich vertieft mit meiner Fragestellungen
                    auseinander zusetzten habe ich mich als ersten Schritt mit den betroffenen direkt ausgetauscht und
                    habe 17 Zuzügler und Zuzüglerinnen von Wiedikon befragt.
                </p>
                <p>
                    In meiner Befragung habe ich darauf abgezielt zu verstehen welche Bedürfnisse neue Bewohner im Kreis
                    3 haben. Zuwanderer die schon länger im Quartier wohnen habe ich über ihr Informationsverhalten, ihr
                    Engagement im Kreis, Tips und Tricks die ihnen geholfen haben als Sie neu im Quartier waren befragt.
                </p>
                <Quote data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
                       data-sal-easing="ease-out-bounce" title="Zitat aus der Befragung">
                    <p>«Profitiert habe ich vor allem von Personen die schon länger hier wohnen und Bescheid wissen was
                        wo läuft»</p>
                </Quote>
                <p>
                    Die Befragungen haben gezeigt dass die Mehrheit der Zuwanderer besonders von Tips und Empfehlungen
                    von Freuenden und einem bestehenden Umfeld profitieren konnten. Nach den persönlichen Empfehlungen
                    ist bei meiner Befragung Facebook am zweit häufigsten erwähnt worden. Da jüngeren vermehrt auf
                    Facebook verzichten, könnten Sie besonders auf die Empfehlungen anderer angewiesen sein.
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

            <chapter title="Recherche">
                <p> Gibt es bereits Lösungen für die Problemstellung? Ich habe mir in einer Recherche folgende Angebote
                    genauer angesehen:
                </p>
                <p>
                    «hellozurich – Das Stadtmagazin»
                    Das Stadtmagazin hat besonders gut aufbereiteten redaktionellen Artikel, meistens in Form von
                    Reportagen. Benutzer haben zudem die Möglichkeiten seine Lieblingsorte zu speichern. Leider kommt
                    dafür der Austausch in einer Community und das Profitieren von anderen Erfahrungen zu kurz.
                </p>
                <p>
                    «AirBnb Erlebnisse» Die Angebote auf AirBnb haben einen Starken Fokus auf Erlebnisse und sind
                    richten sich eher an Touristen die sich für Zürich interessieren. Daher eher unpassend für eine
                    Community des Kreis 3. Dafür lassen sich die Erlebnisse Kommentieren was einen gewissen «Community»
                    Aspekt beinhaltet.
                </p>
                <p>
                    Zusätzlich habe ich mir Applikationen von Überbauungen angesehen, diese verfolgen unteranderem auch
                    das Ziel dass die Nachbarschaft stärker zusammenwächst. Jedoch lag in der App welche ich mir
                    angesehen habe der Fokus klar auf der eigenen Wohnung sowie der Kommunikation zur Bewirtschaftung.
                </p>
            </chapter>

            <chapter title="Ideation">
                <p> Mit den Einblicken die ich durch meine Befragung der Zielgruppe und durch meine eigene Erfahrung
                    gemacht habe sowie einer Recherche was bereits besteht um ähnliche Probleme zu lösen, machte ich
                    mich an die Ideenfindung.
                </p>

                <Quote data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
                       data-sal-easing="ease-out-bounce" title="Linus Pauling">
                    <p>«Der einfachste Weg zu einer guten Idee, ist viele Ideen zu haben.»</p>
                </Quote>

                <p>
                    Eine meiner Lieblingsmethoden dafür ist das «Crazy-8» dabei Zeichnet man 8 Ideen in 8 Minuten. Dabei
                    formten sich mir die Idee eine App zu konzipieren auf der die Bewohner des Kreis 3 ihr Quartier
                    entdecken können und dabei von den Erfahrungen anderer Bewohner profitieren.
                </p>
                <p>
                    Früher hat man sich auf dem Dorfplatz darüber ausgetauscht wo was los ist und dafür soll die App des
                    Kreis 3 eine Moderne alternative bieten. Basierend auf den Interessen des Users werden Ihm
                    Vorschläge gemacht und zeigen so auf wo sich im Quartier das Leben abspielt.
                </p>


            </chapter>
            <g-image src="../assets/img/ideation.jpg"></g-image>


            <chapter title="Benutzerrollen">
                <p> Um meine Zielgruppe besser zu verstehen habe ich 4 Personas entwickelt welche mir dabei helfen die
                    Empathie zur Zielgruppe zu verstärken. Zudem habe ich den Personas eine entsprechende Benutzerrollen
                    in meiner App zugewiesen.
                </p>
                <p>
                    Darf ich vorstellen, das sind Jan Neumann, Valentin Christensen, Larissa Spirituell und Lara
                    Schreiber.
                </p>
            </chapter>

            <Personas data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
                      data-sal-easing="ease-out-bounce">
            </Personas>

            <!--
                        <iframe class="prototype" style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Fproto%2FmAZXKAf5XL25AJiwQECGzP%2FDiplomarbeit%3Fnode-id%3D458%253A0%26viewport%3D125%252C198%252C0.1115327849984169%26scaling%3Dscale-down&chrome=DOCUMENTATION" allowfullscreen></iframe>

                      -->

            <chapter title="User Journey">
                <p>Da ich die Bedürfnisse verschiedner Benutzergruppe auf meiner Plattform abdecken möchte habe ich User
                    Journeys für die Benutzergruppen erstellt. Diese zeigen in schriftlicher Form wie dass User mit
                    einem Bedürfnis die Applikation bedienen würde und wie er durch die App navigiert um zu seinem Ziel
                    zu gelangen.
                </p>
            </chapter>

            <chapter title="Wireframes">
                <p>
                    Die Wireframes basieren auf frühen entwürfen des Konzept und den Flows der User Journeys und
                    enthalten die nötigsten Elemente damit ein User die Applikation bedienen kann. Die Wireframes helfen
                    mir zudem das Konzept zu schärfen und fehlende Details zu ergänzen.
                </p>
            </chapter>

            <Wireframes/>

            <chapter title="Das Konzept">
                <p>
                    Im Onboarding der App werden die eigenen Interessen angegeben. Diese beinhalten Restaurants,
                    Ausgangsmöglichkeiten, Sport, Kunst, Kultur Workshops und vieles mehr.
                </p>
                <p>
                    Basierend auf seinen Interessen werden auf der Startseite, dem «Feed», «Bucketlists» anderer
                    Bewohner deines Quartier angezeigt, diese Bewohner haben also ähnlichen Interessen. In den
                    Bucketlists findet man Kombinierte Orte oder Aktivitäten welche man wiederum auf den eigenen
                    Bucketlists speichern kann.
                </p>
                <p>
                    Anbieter können, nachdem sie sich registriert haben, ein Beitrag ihres Angebot einreichen welches
                    nach einer Überprüfung veröffentlicht wird. Die Bewohner des Kreis 3 können diese Beiträge dann auf
                    ihren «Bucketlists» speichern und mit Beiträgen von anderen Geschäften oder Freizeitaktivitäten
                    kombinieren. Wenn eine Aktivität auf einer Bucketlist gemacht wird, können die Einträge durch eigene
                    Inhalte wie Texte und Bilder angereichert werden so können Tips, Tricks und Erfahrungen an die
                    Community weitergegeben werden.
                </p>
                <p>
                    Neue Bewohner des Kreis 3 haben so die Chance einen Einblick in das Quartier-Leben zu erlangen und
                    können aus den Bucketlists von anderen Ihre eigenen Bucketlists mit neuen Lieblingsorten oder
                    Aktivitäten erstellen.
                </p>
                </p>
            </chapter>

            <chapter title="Testings">
                <p>
                    Während der Erarbeitung habe ich das Konzept in mehreren Feedback-Runden und mit diversen und
                    Usability Testings auf Schwachstellen und Unklarheiten getestet. Dabei konnte ich eine Aussensicht
                    meines Projekt erlangen und habe dabei einige Unklarheiten gefunden:
                <ol>
                    <li>
                        Umfang: Meine ersten Darfst des Konzepts umfasste zu viele Funktionen, besonders da es in diesem
                        Projekt darum geht ein minimum viable product (MVP) Konzept zu entwickeln welches später mit
                        Funktionen, die sich die Community auch wünscht, ausgebaut werden kann.
                        <br>
                        Die vielen Funktionen hatte zur Folge dass das Konzept und das Ziel der App nicht klar
                        verstanden wurde. Als Massnahme dafür habe ich den Funktionsumfang der App bedeutend reduziert
                        und eine klare Abgrenzung gemacht, was die App können soll und was nicht.
                    </li>

                    <li>
                        Lorem ipsom dolor
                    </li>
                </ol>
                </p>
            </chapter>

            <Weekday/>
        </div>
        <Background/>
    </Layout>
</template>

<script>
    import sal from "sal.js";

    import welcome from "../components/welcome"
    import Chapter from "../components/chapter"
    import Lead from "../components/lead"
    import Weekday from "../components/weekday"
    import Background from "../components/background.vue"
    import Quote from "../components/Quote.vue"
    import Population from "../components/population.vue";
    import Zuwanderer from "../components/zuwanderer.vue";
    import Personas from "../components/personas.vue";
    import Wireframes from "../components/wireframes.vue";

    export default {
        metaInfo: {
            title: 'Kreis 3',
            meta: [
                {name: 'author', content: 'Matthias Koch'}
            ],
        },
        components: {
            Zuwanderer,
            Population,
            welcome,
            Chapter,
            Lead,
            Weekday,
            Background,
            Quote,
            Personas,
            Wireframes
        },

        mounted() {
            this.$nextTick(() => sal());
        },

    }
</script>

<style>
    html {
        overflow-x: hidden;
    }

    li {
        margin-top: 1.75rem;
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

    .prototype {
        margin-top: 4rem;
    }

</style>
