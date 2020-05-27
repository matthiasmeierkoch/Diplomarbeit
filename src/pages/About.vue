<template>
    <Layout>
        <AboutBackground/>
        <Leftstage title="So lebt der Kreis 3">
            <p>Profitiere von Tipps und Tricks anderer Bewohner des Kreis 3 und entdecke deinen Kreis jeden Tag neu.
            </p>
        </Leftstage>
    </Layout>
</template>

<script>
    import sal from 'sal.js';
    import Leftstage from "../components/leftstage.vue";
    import AboutBackground from "../components/aboutbackground.vue";

    export default {
        metaInfo: {
            title: 'Kreis 3 App'
        },
        components: {
            AboutBackground,
            Leftstage
        },
        props: ['title'],
        mounted() {
            this.$nextTick(() => sal());
        }
    }
</script>
