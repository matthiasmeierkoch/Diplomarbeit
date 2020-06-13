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
                <p class="quelle__name">¹ Quelle:
                    <a
                            href="https://www.tagesanzeiger.ch/zuerich/stadt/die-grosse-zuercher-zuwanderungsstatistik/story/18344973">
                        Tages Anzeiger, Die grosse Zürcher Zuwanderungsstatistik
                    </a>
                </p>
            </lead>

            <chapter title="Einleitung">
                <p> Wie integriere ich mich möglichst schnell und einfach in ein bestehendes Quartierleben? Und wie kann
                    ich mein Quartier, in dem ich schon länger wohne, noch besser kennenlernen?
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
                <Population data-sal="slide-up"
                            data-sal-delay="100"
                            data-sal-duration="1000"
                            data-sal-easing="ease-out-bounce"
                            title="Bevölkerung Stadt Zürich 2019"></Population>
            </div>

            <p class="comment__map2">
                Im Jahr 2019 war der Kreis 3 der am drittmeisten Zuzüger von anderen Kreisen der Stadt Zürich
                verzeichnete.
            </p>

            <div>
                <Zuwanderer data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
                            data-sal-easing="ease-out-bounce"
                            title="Zuwanderer aus einem anderen Kreis 2019"></Zuwanderer>
            </div>

            <chapter title="Befragung">
                <p>
                    Besonders weil ich einen persönlichen Bezug zu diesem Thema habe, ich bin selber neu in den Kreis 3
                    gezogen, war es mir wichtig, in meiner Erarbeitung objektive Entscheidungen zu treffen und diese,
                    wenn immer möglich, auf Daten zu stützen. Daher und auch um mich vertieft mit meiner Fragestellung
                    auseinander zusetzten, habe ich mich in einem ersten Schritt mit den Betroffenen direkt ausgetauscht
                    und 17 Zuzüger und Zuzügerinnen vom Kreis 3 diesbezüglich befragt.
                </p>
                <p>
                    In meiner Befragung habe ich darauf abgezielt zu verstehen, welche Bedürfnisse neue Bewohner im
                    Kreis 3 haben. Bewohner, die schon länger im Quartier wohnen, habe ich über ihr
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
                    bei meiner Befragung Facebook am zweithäufigsten erwähnt worden. Davon ausgegangen dass jüngere
                    Personen vermehrt auf
                    Facebook verzichten, was <a href="https://www.emarketer.com/content/global-facebook-users-2019"
                                                target="_blank">eine
                    Studie von eMarketer</a> besagt, sind sie besonders auf die Empfehlungen anderer Personen
                    angewiesen.
                </p>
                <g-image data-sal="slide-up"
                         data-sal-delay="100"
                         data-sal-duration="1000"
                         data-sal-easing="ease-out-bounce"
                         src="../assets/img/Facebook_Agegroup.png">
                </g-image>
                <p>Eigene Abbildung basierend auf den Daten von <a
                        href="https://sproutsocial.com/insights/new-social-media-demographics/#FB-demos"
                        target="_blank">Sprout
                    Social</a></p>


                <g-image data-sal="slide-up"
                         data-sal-delay="100"
                         data-sal-duration="1000"
                         data-sal-easing="ease-out-bounce"
                         src="../assets/img/Freizeitangebote.png">
                </g-image>
                <p>
                    Ebenfalls habe ich in der Befragung herausgefunden dass die Mehrheit der Befragten dazu bereit sind
                    eigene Angebote in Form von Workshops, Deutschkursen oder Nachhilfe anzubieten.
                </p>
                <g-image data-sal="slide-up"
                         data-sal-delay="100"
                         data-sal-duration="1000"
                         data-sal-easing="ease-out-bounce"
                         src="../assets/img/Bereitschaft.png">
                </g-image>
                <p>
                    Alle Antworten der Umfrage als CSV:
                    <a class="home-links" href="/Umfrage.csv">Download
                    </a>
                </p>
            </chapter>

            <chapter title="Recherche">
                <p> Gibt es bereits Lösungen für die Problemstellung? Ich habe mir in einer Recherche folgende Angebote
                    genauer angesehen:
                </p>

                <g-image data-sal="slide-up"
                         data-sal-delay="100"
                         data-sal-duration="1000"
                         data-sal-easing="ease-out-bounce"
                         class="recherche"
                         src="../assets/img/hellozurich.png">
                </g-image>
                <p>
                    <a href="https://www.hellozurich.ch/de">«hellozurich – Das Stadtmagazin»</a><br>
                    Das Stadtmagazin hat besonders gut aufbereitete redaktionelle Artikel, meistens in Form von
                    Reportagen. Benutzer haben die Möglichkeit unter anderem die Lieblingsorte der Redaktion zu
                    speichern. Leider kommt dafür der Austausch in der Gemeinschaft (Community) und das Profitieren von
                    den Erfahrungen anderen zu kurz.
                </p>
                <p><b>Pro:</b></p>
                <ul>
                    <li>Qualität der Beiträge</li>
                    <li>Merkliste</li>
                    <li>Kartenansicht</li>
                </ul>

                <p><b>Kontra:</b></p>
                <ul>
                    <li>Kein Austausch innerhalb der Gemeinschaft</li>
                    <li>Keine eigenen Beiträge</li>
                </ul>

                <g-image data-sal="slide-up"
                         data-sal-delay="100"
                         data-sal-duration="1000"
                         data-sal-easing="ease-out-bounce"
                         class="recherche"
                         src="../assets/img/AirBnB.png">
                </g-image>
                <p>
                    <a href="https://www.airbnb.ch/s/experiences" target="_blank">«AirBnb Erlebnisse»</a><br>
                    Die Angebote auf AirBnb haben einen starken Fokus auf Erlebnisse und richten sich hauptsächlich an
                    Touristen, die sich für die Stadt Zürich interessieren. Aus diesem Grund eher unpassend für eine
                    Community des Kreis 3. Dafür lassen sich die Erlebnisse kommentieren, was einen gewissen «Community»
                    Aspekt beinhaltet.
                </p>

                <p><b>Pro:</b></p>
                <ul>
                    <li>Du kannst selber auch ein Anbieter sein</li>
                    <li>Kommentare auf den Erlebnissen</li>
                </ul>

                <p><b>Kontra:</b></p>
                <ul>
                    <li>Tourismus orientiert und daher ungeeignet für eine lokale Gemeinschaft</li>
                </ul>


                <g-image data-sal="slide-up"
                         data-sal-delay="100"
                         data-sal-duration="1000"
                         data-sal-easing="ease-out-bounce"
                         class="recherche"
                         src="../assets/img/Allthings.png">
                </g-image>
                <p>
                    Zusätzlich habe ich mir die App <a
                        href="https://www.allthings.me/de/wohnungswirtschaft">«Allthings»</a> aus der Immobilienbranche
                    angesehen, diese verfolgt unter anderem auch das Ziel,
                    dass die Nachbarschaft stärker zusammenwächst. Durch die Begrenzung auf die Nachbarschaft innerhalb
                    der Überbauung ist die Gemeinschaft allerdings sehr klein und eingeschränkt. Der Fokus dieser App
                    lag jedoch auch
                    auf der eigenen Wohnung, sowie der Kommunikation zur Bewirtschaftung der Überbauung.
                </p>

                <p><b>Pro:</b></p>
                <ul>
                    <li>Unterstützt die Bildung einer Gemeinschaft</li>
                    <li>Eigenes inserieren</li>
                </ul>

                <p><b>Kontra:</b></p>
                <ul>
                    <li>Die Gemeinschaft ist sehr klein</li>
                    <li>Fokus liegt eher auf der Kommunikation zur Immobilienverwaltung</li>
                </ul>
            </chapter>


            <chapter title="Ideation">
                <p>
                    Mit den Einblicken, die ich durch meine Befragung der Zielgruppe und durch meine eigenen Erfahrungen
                    gemacht habe sowie einer Recherche, was bereits besteht um ähnliche Probleme zu lösen, machte ich
                    mich an die Ideenfindung.
                </p>

                <Quote data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
                       data-sal-easing="ease-out-bounce" title="Linus Pauling">
                    <p>«Der einfachste Weg zu einer guten Idee, ist, viele Ideen zu haben.»</p>
                </Quote>

                <p>
                    Eine meiner Lieblingsmethoden dafür ist die <a
                        href="https://blog.prototypr.io/how-to-run-a-crazy-eights-workshop-60d0a67b29a" target="_blank">«Crazy-8-Methode»</a>:
                    man faltet ein Blatt Papier 1x in die horizontale Hälfte und 2x in die vertikale Hälfte, so
                    entstehen acht Flächen. In diese Flächen werden 8 Ideen in 8 Minuten gezeichnet (pro Idee eine
                    Minute).
                </p>
                <p>
                    Dabei formte sich mir die Idee einer Sammlung von Informationen zu gestalten. Darin sollten
                    möglichst alle Informationen zum Kreis 3 beinhaltet sein; Restaurants, Bars, Clubs, Vereine aber
                    auch Informationen zum Abfall und Recyclingsystem im Kreis 3 ect. Zusätzlich im Fokus sollte ja die
                    Gemeinschaft sein und aus diesem Grund habe ich in den ersten Entwürfen ein digitales schwarzes
                    Brett angedacht, auf welchem die Bewohner inserieren und auf die Inserate anderer antworten können,
                    entweder in Form eines Kommentar oder als Privatnachricht.
                </p>


            </chapter>
            <g-image class="content__image" src="../assets/img/ideation.jpg"></g-image>


            <chapter title="Personas">
                <p>
                    Um meine Zielgruppe besser zu verstehen, habe ich 4 Personas entwickelt, welche mir dabei helfen,
                    die Empathie der Zielgruppe zu verstärken. Zudem habe ich den Personas eine entsprechende
                    Benutzerrolle in meiner App zugewiesen.
                </p>
                <p>
                    Darf ich vorstellen: Jan Neumann, Valentin Christen, Larissa Spirituell und Lara Schreiber.
                </p>
                <p>
                    <b>Jan Neumann:</b> Er ist der Neue im Quartier, er möchte sich mit seinen Freunden im Kreis 3
                    integrieren.
                </p>
                <p>
                    <b>Valentin Christen:</b> Er ist schon einige Jahre im Quartier zuhause und nutzt die App um Neues
                    in seinem Quartier zu entdecken. Er möchte zu den ersten gehören, die die neusten Trends entdecken.
                </p>
                <p>
                    <b>Larissa Spirituell:</b> Sie ist Besitzerin einer neuen Yogaschule im Kreis 3 und sie nutzt die
                    App um Schnupperlektionen ihrer Yogaschule zu inserieren und erhofft sich dadurch mehr Besucher in
                    ihren regulären Klassen.
                </p>
                <p>
                    <b>Lara Schreiber:</b> Sie ist freischaffende Journalistin, in ihrer Freizeit schreibt sie gerne
                    Erfahrungsberichte von Kaffees und Restaurants, die sie besucht hat und veröffentlicht diese in der
                    App.
                </p>
            </chapter>

            <Personas>
            </Personas>


            <chapter title="User Journey und Wireframes">
                <p>
                    Da ich die Bedürfnisse verschiedener Benutzergruppe auf meiner Plattform abdecken möchte, habe ich
                    User Journeys für die Benutzergruppen erstellt. Diese zeigen in schriftlicher Form, wie dass der
                    User mit einem Bedürfnis, die App bedient und wie er durch die App navigiert, um zu seinem Ziel zu
                    gelangen.
                </p>

                <p>
                    Die Wireframes sind Konzeptentwürfe, die aus den Flows der User Journeys entstanden sind. Darauf zu
                    sehen sind alle nötigen Elemente damit ein User die Applikation bedienen kann. Die Wireframes helfen
                    zu verstehen ob die Idee als Konzept funktioniert.
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
                    Meine ersten Entwürfe des Konzepts umfassten zu viele Funktionen, das Konzept soll schlüssig sein um
                    ein minimum viable product <a href="https://de.wikipedia.org/wiki/Minimum_Viable_Product"
                                                  target="_blank">(MVP)</a> Produkt zu entwickeln, welches zu einem
                    späteren Zeitpunkt immer noch mit zusätzlichen Funktionen ausgebaut werden kann.
                </p>
                <p>
                    Die vielen Funktionen hatten zur Folge, dass das Ziel der App nicht klar verstanden wurde. Als
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
                    Die App soll den Bewohnenden des Kreis 3 ermöglichen, ihr Quartier (neu) zu entdecken und sich in
                    der Gemeinschaft einzubringen. Der natürlichste Weg sich nachhaltig zu integrieren ist das
                    gemeinsame Erleben. Dies machen sie, indem sie Angebote inserieren oder an inserierten Angeboten
                    anderer Benutzer teilnehmen.
                </p>
                <p>
                    Früher hat man sich auf dem Dorfplatz darüber ausgetauscht, wo was und wann los ist. Dafür soll
                    die App des Kreis 3 eine moderne Alternative bieten. Basierend auf den Interessen des Users werden
                    ihm Vorschläge aufgezeigt, was er unternehmen kann (Freizeitangebote, Veranstaltungen, Sport,
                    Restaurantvorschläge ect.).
                </p>
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

            <Konzept/>

            <Chapter title="Design">
                <p>
                    In einer Feedbackrunde bekam ich eine kritische Rückmeldung zum Entwurf meines ersten Designs. Der
                    erste Entwurf hatte sehr wenig Charakter und war ein schlichtes «Flat Design». Meine erste
                    Schriftwahl, die auf Google Fonts angebotene «Inter», hatte sich auch nicht besonders mit der
                    Thematik meiner Arbeit gedeckt. Aus diesem Grund habe ich dann nach einer lokalen, schweizer Schrift
                    gesucht mit mehr Charakter. Ich habe mich für eine Kombination einer Serifenschrift, die «Suisse
                    Neue» und der Sans Serif «Suisse BP int'l» von <a href="https://www.swisstypefaces.com/"
                                                                      target="_blank">Swiss Typefaces</a> entschieden.
                </p>
                <p>
                    Weiter habe ich mich für eine Farbpalette entschieden, welche freundlich, einladend und modern sein
                    soll und der App einen emotionalen Charakter verleiht.

                </p>
                <g-image data-sal="slide-up"
                         data-sal-delay="100"
                         data-sal-duration="1000"
                         data-sal-easing="ease-out-bounce"
                         src="../assets/img/DesignEntwicklung.png">
                </g-image>
                <p>
                    Das Design System meiner App ist auf einem 8px Grid aufgebaut, d.h. alle Abstände lassen sich durch
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

            <chapter>
                <h3>Designentscheidungen</h3>
                <p>
                    Einige Entscheidungen, die ich im Design und Konzept getroffen haben möchte ich besonders
                    hervorheben. Dieses Konzept wurde am Beispiel des Kreis 3 konzipiert, das Konzept könnte sehr gut
                    auch auf weitere Kreise oder sogar auf die gesamte Stadt erweitert werden. Da zur Zeit der Fokus des
                    Konzepts auf einem Kreis liegt, habe ich mich gegen den Einsatz einer Karte entschieden, da sich die
                    Aktivitäten meistens in Gehdistanz befinden.
                </p>
                <p>
                    Auch wenn es sich positiv auf das bilden einer Gemeinschaft auswirken könnte, habe ich mich gegen
                    eine Nachrichten Funktion innerhalb der App entschieden. Der Grund dafür ist, dass die Aktivitäten
                    auf der App möglichst offen angeboten werden sollen, ohne dass eine «Vorauswahl» via Nachrichten
                    stattfindet. Zudem war es mir wichtig, dass sich die App nicht in die Richtung einer «Dating-App»
                    entwickelt. Die Gemeinschaft wird durch das gemeinsame Erleben von Aktivitäten gestärkt.
                </p>
                <p>
                    In der App wird das Wort «Bucketlist» verwendet. Dies steht für die Listen von gespeicherten
                    Beiträgen. Ich habe mich hier bewusst für das englische Wort entschieden. Das Wort “Bucketlist” wird
                    oft im Zusammenhang mit Reisen und Erleben verwendet und aus diesem Grund schien es mir für meinen
                    Verwendungszweck sehr passend.
                </p>
                <p>
                    Das Konzept stützt sich stark auf die in meiner Umfrage gewonnenen Erkenntnisse, dass die Mehrheit
                    der Befragten nicht sehr engagiert im Kreis sind, jedoch sind sie dazu bereit, sich stärker zu
                    engagieren. Zudem können die Zuzügelnden von dem Wissen der bestehenden Gemeinschaft profitieren.
                </p>
                <div class="button__next">
                    <g-link to="/about/">Zur Kreis 3 App</g-link>
                </div>
            </chapter>

            <chapter title="Prototyp"
                     data-sal="slide-up"
                     data-sal-delay="100"
                     data-sal-duration="1000"
                     data-sal-easing="ease-out-bounce"
                     class="prototype">
            </chapter>
            <iframe data-sal="slide-up"
                    data-sal-delay="100"
                    data-sal-duration="1000"
                    data-sal-easing="ease-out-bounce"
                    style="border: 1px solid rgba(0, 0, 0, 0.1);" width="100%" height="600"
                    src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Fproto%2FmAZXKAf5XL25AJiwQECGzP%2FDiplomarbeit%3Fnode-id%3D791%253A1966%26viewport%3D-1500%252C-483%252C0.3589903712272644%26scaling%3Dscale-down&chrome=DOCUMENTATION"
                    allowfullscreen></iframe>


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
            Konzept
        },

        mounted() {
            this.$nextTick(() => sal({
                threshold: 0.2
            }));
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

    ol {
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

    .content__image {
        border-radius: 1rem;
    }

    .button__next {
        background-color: #E4665C;
        font-weight: bold;
        color: white;
        padding: 1rem;
        text-align: center;
        border-radius: 2rem;
        max-width: 50%;
        margin: auto;
        margin-top: 4rem;
    }

    .button__next :visited {
        color: white;
    }

    .button__next :link{
        text-decoration: none;
    }

    .button__next :hover {
        text-decoration: underline;
    }

    svg {
        padding-top: 0.5rem;
    }


    img {
        width: 100%;
    }

    .recherche {
        border-radius: 1rem;
        width: 75%;
        margin-left: 12.5%;
        margin-top: 2rem;
        margin-bottom: 1.5rem;
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

    @media (max-width: 420px) {
        .comment__map2 {
            margin-left: 1rem;
        }

        .recherche {
            width: 100%;
            margin: auto;
            margin-top: 2rem;
        }
    }

    @media (max-width: 420px) {
        .prototype {
            visibility: hidden;
        }
    }

</style>
