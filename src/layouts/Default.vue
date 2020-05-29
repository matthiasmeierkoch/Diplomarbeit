<template>

    <div class="layout">
        <Navigation/>
        <slot/>
    </div>

</template>

<static-query>
    query {
    metadata {
    siteName
    }
    }
</static-query>

<script>
    import sal from 'sal.js';
    import Navigation from "../components/navigation.vue"

    export default {
        components: {
            Navigation
        },

        mounted() {
            this.$nextTick(() => sal());
        }

    }

</script>

<style>
    @import "../../node_modules/sal.js/dist/sal.css";

    html{
        overflow-x: hidden;
    }

    @font-face {
        font-family: "Suisse Neue";
        src: url(../assets/font/SuisseNeue-Medium-WebS.woff);
    }

    @font-face {
        font-family: "Suisse BP Int";
        src: url(../assets/font/SuisseIntl-Regular-WebS.woff);
    }

    @font-face {
        font-family: "SangBleu";
        src: url(../assets/font/SangBleuRepublic-Bold-WebS.woff);
    }

    body {
        font-family: "Suisse BP Int", system-ui, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
        padding: 0;
        line-height: 1.5;
        background: #EFE8DC;
        background-size: auto;
    }

    .layout {
        max-width: 1110px;
        margin: 0 auto;
        padding-left: 30px;
        padding-right: 30px;
    }

    @media (max-width: 768px) {
        .layout{
            padding-left: 16px;
            padding-right: 16px;

        }
    }
</style>
