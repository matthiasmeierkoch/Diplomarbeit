<template>

    <div class="welcome" data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
         data-sal-easing="ease-out-bounce">
        <h1 class="project__title">Willkommen im Kreis 3</h1>
        <div class="welcome__subtitle">
            <p class="welcome__subtitle">Eine Arbeit über die Integration in ein bestehendes Quartierleben anhand des Kreis 3 in Zürich</p>
        </div>
    </div>

</template>

<script>
    import sal from "sal.js";

    export default {
        name: "welcome",

        mounted() {
            this.$nextTick(() => sal());
        }
    }
</script>

<style scoped>

    .welcome{
        margin-left: auto;
        margin-right: auto;
        margin-bottom: 5rem;
        text-align: center;
        z-index: 10;
    }

    .project__title {

    }

    .welcome__subtitle {
        width: 90%;
        font-size: 2rem;
        line-height: 3rem;
        color: #ffffff;
        margin: auto;
    }

    .project__title {
        font-size: 6.5rem;
        line-height: 7.3rem;
        margin-top: 35vh;
        width: 100%;
        text-align: center;
        color: #ffffff;
        font-family: "SangBleu";
    }


    @media (max-width: 768px) {
        .project__title {
            font-size: 4rem;
            width: 100%;
            line-height: 4rem;
            margin-top: 20vh;
        }

        .project__subtitle {
            width: 100%;
        }
    }

    @media (max-width: 420px) {
        .project__title {
            font-size: 3rem;
            width: 100%;
            line-height: 4rem;
            margin-top: 35vh;
        }

        .welcome__subtitle {
            width: 100%;
            font-size: 1.5rem;
            line-height: 2rem;
        }
    }
</style>