<template>
    <Layout>
        <!-- Learn how to use images here: https://gridsome.org/docs/images -->
        <div class="container">
            <welcome/>

            <lead>
                <p> In den letzten 10 Jahren sind zwischen 41&#x202F;000 und 46&#x202F;000 Personen pro Jahr nach Zürich
                    gezogen.¹ Für viele ist ein Umzug und besonders ein Kantons- oder sogar Landeswechsel immer auch mit
                    Komplikationen und Unsicherheiten verbunden.
                </p>
                <p class="quelle__name"> ¹ Quelle:
                    <a
                            href="https://www.tagesanzeiger.ch/zuerich/stadt/die-grosse-zuercher-zuwanderungsstatistik/story/18344973">
                        Tages Anzeiger, Die grosse Zürcher Zuwanderungsstatistik
                    </a>
                </p>
            </lead>

            <chapter title="Einleitung">
                <p> Wie integriere ich mich möglichst schnell und einfach in ein bestehendes Quartierleben? Und wie kann
                    ich mein Quartier, in dem ich schön länger wohne, noch besser kennenlernen?
                </p>
                <p>
                    Mit diesen Problemstellungen habe ich mich in meiner Diplomarbeit auseinandergesetzt. In meiner
                    Arbeit habe ich dabei den Kreis 3 der Stadt Zürich als Beispiel genommen. Zur Lösung der
                    Problemstellung im Kreis 3 habe ich eine App konzipiert und gestaltet, welche neuen und bestehenden
                    Bewohner des Kreis 3 ermöglicht, diesen zu entdecken und sich in der Gemeinschaft mit einzubringen.
                </p>
                <p>
                    Der Kreis 3 umfasst die Quartiere: Sihlfeld, Alt-Wiedikon und Friesenberg. 2019 lebten etwas über
                    45&#x202F;000 Personen im Kreis 3, damit ist er der am zweitstärksten bevölkerte Kreis in der Stadt
                    Zürich.
                </p>
            </chapter>

            <div>
                <Population data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
                            data-sal-easing="ease-out-bounce" title="Bevölkerung Stadt Zürich 2019"></Population>
            </div>

            <p class="comment__map2">
                Im Jahr 2019 war der Kreis 3 der am drittmeisten Zuzüger von anderen Kreisen der Stadt Zürich
                verzeichnete.
            </p>

            <div>
                <Zuwanderer data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
                            data-sal-easing="ease-out-bounce"
                            title="Zuwanderer aus einem anderen Kreis 2019"></Zuwanderer>
            </div>

            <chapter title="Befragung">
                <p> Besonders weil ich einen persönlichen Bezug zu diesem Thema habe, ich bin selber neu in den Kreis 3
                    gezogen, war es mir wichtig, in meiner Erarbeitung objektive Entscheidungen zu treffen und diese,
                    wenn immer möglich, auf Daten zu stützen. Daher und auch um mich vertieft mit meiner Fragestellung
                    auseinander zusetzten, habe ich mich als ersten Schritt mit den betroffenen direkt ausgetauscht und
                    habe 17 Zuzüger und Zuzügerinnen vom Kreis 3 diesbezüglich befragt.
                </p>
                <p>
                    In meiner Befragung habe ich darauf abgezielt zu verstehen welche Bedürfnisse neue Bewohner im Kreis
                    3 haben. Zuwanderer die schon länger im Quartier wohnen habe ich über ihr Informationsverhalten, ihr
                    Engagement im Kreis, Tips und Tricks die ihnen geholfen haben als Sie neu im Quartier waren befragt.
                </p>
                <p>
                    In meiner Befragung habe ich darauf abgezielt zu verstehen, welche Bedürfnisse neue Bewohner im
                    Kreis 3 haben. Bewohner, die schon länger im Quartier wohnen, habe ich über ihr
                    Informationsverhalten, ihr Engagement im Kreis, Tipps und Tricks, die ihnen geholfen haben, als sie
                    selber neu im Kreis waren, befragt.
                </p>
                <Quote data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
                       data-sal-easing="ease-out-bounce" title="Zitat aus der Befragung">
                    <p>«Profitiert habe ich vor allem von Personen die schon länger hier wohnen und Bescheid wissen was
                        wo läuft»</p>
                </Quote>
                <p>
                    Die Befragung hat gezeigt, dass die Mehrheit der Zuwanderer besonders von Tipps und Empfehlungen von
                    Freunden und einem bestehenden Umfeld profitieren konnten. Nach den persönlichen Empfehlungen ist
                    bei meiner Befragung Facebook am zweithäufigsten erwähnt worden. Da jüngere Personen vermehrt auf
                    Facebook verzichten, sind sie besonders auf die Empfehlungen anderer Personen angewiesen.
                </p>
                <p>
                    Alle Daten als CSV:
                    <a class="home-links" href="/Umfrage.csv"> Download
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
                    <a href="https://www.hellozurich.ch/de">«hellozurich – Das Stadtmagazin»</a><br>
                    Das Stadtmagazin hat besonders gut aufbereitete redaktionelle Artikel, meistens in Form von
                    Reportagen. Benutzer haben die Möglichkeit unter anderem die Lieblingsorte der Redaktion zu
                    speichern. Leider kommt dafür der Austausch in der Gemeinschaft (Community) und das Profitieren von
                    den Erfahrungen anderen zu kurz.
                </p>
                <p>
                    <a href="https://www.airbnb.ch/s/experiences">«AirBnb Erlebnisse»</a><br>
                    Die Angebote auf AirBnb haben einen starken Fokus auf Erlebnisse und richten sich hauptsächlich an
                    Touristen, die sich für die Stadt Zürich interessieren. Aus diesem Grund eher unpassend für eine
                    Community des Kreis 3. Dafür lassen sich die Erlebnisse kommentieren, was einen gewissen «Community»
                    Aspekt beinhaltet.

                </p>
                <p>
                    Zusätzlich habe ich mir Apps wie <a
                        href="https://www.allthings.me/de/wohnungswirtschaft">Allthings</a> aus der Immobilienbranche
                    angesehen, diese verfolgen unter anderem auch das Ziel,
                    dass die Nachbarschaft stärker zusammenwächst. Durch die Begrenzung auf die Nachbarschaft innerhalb
                    der Überbauung ist die Community sehr klein und eingeschränkt. Der Fokus dieser Apps lag jedoch ganz
                    klar auf den eigenen Wohnungen sowie der Kommunikation zur Bewirtschaftung der Überbauung.
                </p>
            </chapter>

            <chapter title="Ideation">
                <p> Mit den Einblicken, die ich durch meine Befragung der Zielgruppe und durch meine eigenen Erfahrungen
                    gemacht habe sowie einer Recherche, was bereits besteht um ähnliche Probleme zu lösen, machte ich
                    mich an die Ideenfindung.
                </p>

                <Quote data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
                       data-sal-easing="ease-out-bounce" title="Linus Pauling">
                    <p>«Der einfachste Weg zu einer guten Idee, ist, viele Ideen zu haben.»</p>
                </Quote>

                <p>
                    Eine meiner Lieblingsmethoden dafür ist die «Crazy-8-Methode»: man zeichnet 8 Ideen in 8 Minuten.
                    Dabei formte sich mir die Idee eine App zu konzipieren, auf der die Bewohner des Kreis 3 ihr
                    Quartier (neu) entdecken und sich in der Gemeinschaft einbringen können. Dies machen sie indem sie
                    Angebote inserieren oder an inserierten Angeboten anderer Benutzer teilnehmen.
                </p>
                <p>
                    Früher hat man sich auf dem Dorfplatz darüber ausgetauscht, wo was und wann los ist. Dafür soll die
                    App des Kreis 3 eine moderne Alternative bieten. Basierend auf den Interessen des Users werden ihm
                    Vorschläge aufgezeigt was er unternehmen kann (Freizeitangebote, Veranstaltungen, Sport,
                    Restaurantvorschläge ect.).
                </p>


            </chapter>
            <g-image src="../assets/img/ideation.jpg"></g-image>


            <chapter title="Personas">
                <p>
                    Um meine Zielgruppe besser zu verstehen, habe ich 4 Personas entwickelt, welche mir dabei helfen,
                    die Empathie zur Zielgruppe zu verstärken. Zudem habe ich den Personas eine entsprechende
                    Benutzerrolle in meiner App zugewiesen.
                </p>
                <p>
                    Darf ich vorstellen, das sind Jan Neumann, Valentin Christen, Larissa Spirituell und Lara Schreiber.
                </p>
            </chapter>

            <Personas
                    data-sal="slide-up"
                    data-sal-delay="100"
                    data-sal-duration="1000"
                    data-sal-easing="ease-out-bounce">
            </Personas>


            <chapter title="User Journey und Wireframes">
                <p>
                    Da ich die Bedürfnisse verschiedener Benutzergruppe auf meiner Plattform abdecken möchte, habe ich
                    User Journeys für die Benutzergruppen erstellt. Diese zeigen in schriftlicher Form, wie dass der
                    User mit einem Bedürfnis die App bedient und wie er durch die App navigiert, um zu seinem Ziel zu
                    gelangen.
                </p>

                <p>
                    Die Wireframes sind Konzeptentwürfe, die aus den Flows der User Journeys entstanden sind. Darauf zu
                    sehen sind alle nötigen Elemente damit ein User die Applikation bedienen kann.
                </p>
            </chapter>

            <Wireframes
                    data-sal="slide-up"
                    data-sal-delay="100"
                    data-sal-duration="1000"
                    data-sal-easing="ease-out-bounce">
            </Wireframes>

            <chapter title="Testings">
                <p>
                    Während der Erarbeitung habe ich das Konzept in mehreren Feedback-Runden und mit mehreren Usability
                    Testings auf Schwachstellen und Unklarheiten getestet. Dabei konnte ich eine Aussensicht meines
                    Projekts erlangen und habe dabei einige Unklarheiten gefunden, welche hauptsächlich auf den zu
                    grossen Funktionsumfang zurückzuführen waren.
                </p>
                <p>
                    Meine ersten Entwürfe des Konzepts umfassten zu viele Funktionen, das Konzept soll ein schlüssig
                    sein um ein minimum viable product (MVP) Produkt zu entwickeln welches zu einem späteren Zeitpunkt
                    immer noch ausgebaut werden kann.
                </p>
                <p>
                    Die vielen Funktionen hatte zur Folge, dass das Ziel der App nicht klar verstanden wurde. Als
                    Massnahme dafür habe ich den Funktionsumfang der App bedeutend auf das Wesentliche reduziert und
                    eine klare Abgrenzung gemacht, was die App kann und was nicht.
                </p>

                <div style="margin-top: 4rem"></div>
                <p>Auf der App können...</p>
                <ol>
                    <li>
                        ...Aktivitäten und Geschäfte entdeckt werden.
                    </li>
                    <li>
                        ...Aktivitäten und Geschäfte gespeichert werden.
                    </li>
                    <li>
                        ...Aktivitäten und Geschäfte inseriert werden.
                    </li>
                    <li>
                        ...angesehen werden was andere erlebt haben.
                    </li>
                    <li>
                        ...eigene Erfahrungen mit Community geteilt werden.
                    </li>
                </ol>
                <div style="margin-top: 4rem"></div>
                <p>Innerhalb der App können keine...</p>
                <ol>
                    <li>
                        ...Nachrichten empfangen oder versendet werden.
                    </li>
                    <li>
                        ...keinen Personen «gefolgt» werden.
                    </li>
                    <li>
                        ...keine kantonale / administrative Informationen gefunden werden.
                    </li>
                </ol>
                <div style="margin-top: 4rem"></div>
                <p>
                    Als Folge der Usability Testings habe ich die Navigation angepasst um die Priorisierung meiner
                    Fragestellung stärker in den Fokus zu bringen.
                </p>
                <g-image
                        data-sal="slide-up"
                        data-sal-delay="100"
                        data-sal-duration="1000"
                        data-sal-easing="ease-out-bounce"
                        src="../assets/img/Navigation.png"></g-image>
            </chapter>

            <chapter title="Das Konzept">
                <p>
                    Im Onboarding der App werden die eigenen Interessen angegeben. Diese beinhalten Restaurants,
                    Ausgangsmöglichkeiten, Sport, Kunst, Kultur, Workshops und vieles mehr.
                </p>
                <p>
                    Basierend auf den angegebenen Interessen werden auf der Startseite diverse, passende Angebote im
                    Kreis 3 angezeigt. Gefällt einem ein Angebot kann dieses auf seiner Bucketlist gespeichert werden.

                </p>
                <p>
                    Basierend auf den angegebenen Interessen werden auf der Startseite diverse, passende Angebote im
                    Kreis 3 vorgeschlagen. Wie sehr ein Angebot zu einem passt, zeigt ein «Match» in Prozent an. Gefällt
                    einem ein Angebot, kann dieses auf einer Bucketlist gespeichert werden.
                </p>
                <p>
                    Möchte man zum Beispiel eine Yoga-Schnupperlektion anbieten, so kann man, nachdem man sich
                    registriert hat, das eigene Angebot einreichen welches nach einer Überprüfung durch den Kanton
                    Zürich veröffentlicht wird. Die Bewohner des Kreis 3 können diese Beiträge auf ihren «Bucketlists»
                    speichern und mit weiteren Beiträgen kombinieren oder ergänzen. Aktivitäten auf der Bucketlist
                    können als «ich war hier» markiert werden und können zusätzlich durch eigene Inhalte (Texte und
                    Bilder) Tipps und Tricks weitergegeben werden. So können andere Benutzer der App von deinen
                    Erfahrungen profitieren.
                </p>
                <p>
                    Neue Bewohner des Kreis 3 haben so die Chance einen Einblick in das Quartier-Leben zu erlangen und
                    finden für sich passende Aktivitäten. Weiter können sie aus den veröffentlichten Bucketlists von
                    anderen Benutzern ihre eigenen Bucketlists mit Lieblingsorten oder Aktivitäten erstellen.
                </p>
                <p>
                    Der USP (Unique Selling Point) der App ist die Community. Die App muss mehr sein als «nur» ein
                    Verzeichnis, welches aufzeigt wo was ist. Die User sollen aktiv die Möglichkeit haben, passende
                    Beiträge zu entdecken und eigene Beiträge hinzuzufügen. Durch das gemeinsame Erleben wächst die
                    Gemeinschaft auf eine natürliche Art und Weise stärker zusammen.
                </p>
            </chapter>

            <Konzept
                    data-sal="slide-up"
                    data-sal-delay="100"
                    data-sal-duration="1000"
                    data-sal-easing="ease-out-bounce">
            </Konzept>

            <Chapter title="Design">
                <p>
                    Im Design habe ich mich für eine Kombination einer Serifen Schrift, die «Suisse Neue» und der Sans
                    Serif «Suisse BP int'l» entschieden. Dabei war es mir sehr wichtig eine Schweizer Schrift zu
                    verwenden. Ich habe mich für eine Farbpalette entschieden welche freundlich, einladend und modern
                    sein soll.
                </p>
                <p>
                    Das Designsystem meiner App ist auf einem 8px Grid aufgebaut, d.h. alle Abstände lassen sich durch
                    8px teilen. Meine Komponenten bestehen aus diversen Atomen, wie ich diese Unterteilung gemacht habe,
                    ist auf dem Bild weiter unten zu sehen.
                </p>
            </Chapter>
            <Designsystem
                    data-sal="slide-up"
                    data-sal-delay="100"
                    data-sal-duration="1000"
                    data-sal-easing="ease-out-bounce">
            </Designsystem>

            <chapter title="Prototyp"
                     data-sal="slide-up"
                     data-sal-delay="100"
                     data-sal-duration="1000"
                     data-sal-easing="ease-out-bounce"
                     class="prototype">
                <iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450"
                        src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Fproto%2FmAZXKAf5XL25AJiwQECGzP%2FDiplomarbeit%3Fnode-id%3D791%253A1966%26viewport%3D-1500%252C-483%252C0.3589903712272644%26scaling%3Dscale-down&chrome=DOCUMENTATION"
                        allowfullscreen></iframe>
            </chapter>
           <chapter>
            <Thanks/>
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
    import Designsystem from "../components/designsystem.vue";
    import Konzept from "../components/concept.vue";
    import Thanks from "../components/thanks.vue";

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
            Wireframes,
            Designsystem,
            Konzept,
            Thanks
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
        font-size: 1.375rem;
        line-height: 2.0625rem;
        color: #003041;
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

    .quelle__name {
        font-size: 1rem;
        margin-top: -2rem;
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

    .comment__map2 {
        max-width: 50ch;
        margin: 4rem 3rem 2rem;
        font-size: 1.375rem;
        line-height: 2.0625rem;
    }

    @media (min-width: 420px) {
        .prototype{
            visibility: hidden;
        }
        .comment__map2{
            margin: 1.25rem;
        }
    }

</style>
