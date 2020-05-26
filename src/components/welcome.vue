<template>

    <div class="welcome">
        <h1 class="project__title">Willkommen im Kreis 3</h1>
        <div class="project__subtitle">
        </div>
    </div>

</template>

<script>
    export default {
        name: "title"
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
            font-size: 3.65rem;
            max-width: 100%;
            line-height: 4.25rem;
            margin-top: 20vh;
        }

        .project__subtitle {
            width: 100%;
        }
    }
</style>