<template>

    <div class="welcome" data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
         data-sal-easing="ease-out-bounce">
        <h1 class="project__title">Willkommen im Kreis 3</h1>
        <div class="project__subtitle">
        </div>
    </div>

</template>

<script>
    import sal from "sal.js";

    export default {
        name: "title",

        mounted() {
            this.$nextTick(() => sal());
        }
    }
</script>

<style scoped>

    .welcome {
        position: relative;
        margin-top:3rem;
        margin-bottom: 5rem;
    }

    .project__title {
        width: 100%;
        text-align: center;
        color: #ffffff;
        font-family: "SangBleu";
    }

    .project__subtitle {
        width: 100%;
        font-size: 1.375rem;
        line-height: 2.0625rem;
    }

    .project__title {
        font-size: 6.5rem;
        line-height: 7.3rem;
        color: #fff;
        max-width: 43rem;
        margin-top: 25vh;
    }

    @media (max-width: 667px) {

        .project__title {
            font-size: 3.25rem;
            width: 100%;
            line-height:4rem;
            margin-top: 20vh;
        }

        .project__subtitle {
            width: 100%;
        }
    }
</style>