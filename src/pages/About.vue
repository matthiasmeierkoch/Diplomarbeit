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

        <Community>
            <p>Integriere dich in die bestehende Gemeinschaft des Kreis 3 durch das gemeinsame Erleben.</p>
        </Community>

        <Startseite title="Finde was zu dir passt">
            <p>
                Profitiere von Tipps und Tricks anderer Bewohner des Kreis&nbsp;3 und entdecke deinen Kreis jeden Tag
                neu.
            </p>
        </Startseite>

        <Explore title="Neues Entdecken">
            <p>
                Sieh dir an was im Kreis&nbsp;3 erlebt wird und speichere Beiträge die dir gefallen auf deiner eigenen
                Bucketlist.
            </p>
        </Explore>

        <Bucketlist title="Teile deine Erfahrungen">
            <p>
                Teile deine Erfahrungen und deine Lieblingsorte des Kreis&nbsp;3 mit den Bewohnern des Kreis&nbsp;3
                und
                veröffentliche deine Bucketlists.
            </p>
        </Bucketlist>
        <CTA
                data-sal="slide-up"
                data-sal-delay="100"
                data-sal-duration="1000"
                data-sal-easing="ease-out-bounce">
        </CTA>

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
            Community
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
            font-size:1.5rem;
            line-height: 4rem;
        }

    }
</style>
