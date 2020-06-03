<template>
    <Layout>
        <AboutBackground/>
        <Startseite title="Die App des Kreis 3">
            <p>
                Profitiere von Tipps und Tricks anderer Bewohner des Kreis 3 und entdecke deinen Kreis jeden Tag neu.
            </p>
        </Startseite>

        <Explore title="Eine neue Art des Entdeckens">
            <p>
                Sieh dir an was im Kreis 3 erlebt wird und speichere Beiträge die dir gefallen auf deiner eigenen
                Bucketlist.
            </p>
        </Explore>

        <Bucketlist title="Von der Community für die Community">
            <p>
                Teile deine Erfahrungen und deine Lieblingsorte des Kreis 3 mit den Bewohnern des Kreis 3 und
                veröffentliche deine Bucketlists.
            </p>
        </Bucketlist>

    </Layout>
</template>

<script>
    import sal from 'sal.js';
    import Startseite from "../components/aboutstartseite.vue";
    import Explore from "../components/about_explore.vue";
    import Bucketlist from "../components/about_bucketlist.vue";
    import AboutBackground from "../components/aboutbackground.vue";

    export default {
        metaInfo: {
            title: 'Kreis 3 App'
        },
        components: {
            AboutBackground,
            Startseite,
            Explore,
            Bucketlist
        },
        props: ['title'],
        mounted() {
            this.$nextTick(() => sal());
        }
    }
</script>
