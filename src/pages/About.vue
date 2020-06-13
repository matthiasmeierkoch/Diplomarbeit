<template>
    <Layout>
        <div data-sal="slide-up"
             data-sal-delay="100"
             data-sal-duration="1000"
             data-sal-easing="ease-out-bounce"
             class="title__about">
            <h1>Die App des <br>Kreis&nbsp;3</h1>
        </div>

        <g-image data-sal="slide-up"
                 data-sal-delay="100"
                 data-sal-duration="1000"
                 data-sal-easing="ease-out-bounce"
                 class="mockup"
                 src="../assets/img/Mockup.png">
        </g-image>

        <!--        <Community>
                    <p>Integriere dich in die bestehende Gemeinschaft des Kreis 3 durch das gemeinsame Erleben.</p>
                </Community>-->

        <Startseite title="Finde, was du suchst">
            <p>
                Sieh dir an, was der Kreis&nbsp;3 genau für deine Interessen zu bieten hat, und was dir gefällt
                speicherst du auf einer deiner Bucketlists.
            </p>
        </Startseite>

        <Bucketlist title="Teile deine Erfahrungen">
            <p>
                Teile deine Erfahrungen und deine Lieblingsorte des Kreis&nbsp;3 mit der Gemeinschaft,
                indem du Tipps und Tricks in deiner Bucketlist festhältst und diese veröffentlichst.
            </p>
        </Bucketlist>
        <CTA
                data-sal="slide-up"
                data-sal-delay="100"
                data-sal-duration="1000"
                data-sal-easing="ease-out-bounce">
        </CTA>

        <Chapter title="Erkentnisse und Schlusswort">
            <p>
                Ich habe in meiner Diplomarbeit ein Konzept erarbeitet zur Gemeinschaftsbildung des Stadtkreis 3 in
                Zürich. Dabei konnte ich mich vertieft damit auseinandersetzen was es heisst, neu im Kreis 3 zu sein.
                Eine meiner Erkenntnisse dabei war, dass man nicht wirklich lange «neu» in einem Quartier ist, nach
                einigen Wochen kennt man bereits die wichtigsten Punkte zum Quartierleben, ist deswegen aber noch lange
                nicht in der Gemeinschaft integriert.
            </p>
            <p>
                Eine weitere Erkenntnis der Arbeit war, dass eine Integration nicht erzwungen werden kann. Zudem ist
                eine Integration niemals wirklich vollendet und sollte stets fortgeführt werden womit auch die
                Bewohnenden betroffen sind, die schon länger im Kreis 3 leben.
            </p>
            <p>
                Weiter möchte ich hervorheben, dass es die eigene Entscheidung ist, diese soll es auch sein, ob und wie
                sehr man sich integrieren möchte. Aus diesem Grund sollte die Integration möglichst zugänglich gemacht
                werden. Ein Weg, wie diese möglichst zugänglich gemacht werden kann, ist das von mir erarbeitete
                Produkt: die «Kreis 3 App».
            </p>
            <p>
                Vielen Dank für das Interesse an meiner Diplomarbeit.<br><br>
                Matthias Koch
            </p>
        </Chapter>

        <AboutBackground/>

    </Layout>
</template>

<script>
    import sal from 'sal.js';
    import Startseite from "../components/aboutstartseite.vue";
    import Explore from "../components/about_explore.vue";
    import Bucketlist from "../components/about_bucketlist.vue";
    import AboutBackground from "../components/aboutbackground.vue";
    import CTA from "../components/appstore.vue";
    import Community from "../components/community.vue";
    import Chapter from "../components/chapter.vue";

    export default {
        metaInfo: {
            title: 'Kreis 3 App'
        },
        components: {
            AboutBackground,
            Startseite,
            Explore,
            Bucketlist,
            CTA,
            Community,
            Chapter
        },
        props: ['title'],
        mounted() {
            this.$nextTick(() => sal());
        }
    }
</script>

<style>
    .mockup {
        margin-top: 5vh;
        width: 100%;
        position: relative;
    }

    .title__about {
        font-family: "Suisse Neue";
        font-size: 3rem;
        margin: auto;
        color: #003041;
        text-align: center;
        margin-top: 17vh;
    }


    @media (max-width: 780px) {
        .title__about {
            font-size: 1.5rem;
            line-height: 4rem;
        }
    }
</style>
