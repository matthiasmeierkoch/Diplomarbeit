<template>
    <Layout>
        <Leftstage title="So lebt der Kreis 3">
            <p>Die Kreis 3 App ist ein soziales Netzwerk für alle Bewohner des Kreis 3. Mithilfe
                dieser App können sich neue Bewohner schneller integrieren und besser einleben und von Tipps anderer
                Kreis 3 Bewohner profitieren.
            </p>
        </Leftstage>
    </Layout>
</template>

<script>
    import sal from 'sal.js';
    import Leftstage from "../components/leftstage";

    export default {
      metaInfo: {
        title: 'Kreis 3 App'
      },
      components: {
        Leftstage
      },
      props: ['title'],
      mounted() {
        this.$nextTick(() => sal());
      }
    }
</script>
