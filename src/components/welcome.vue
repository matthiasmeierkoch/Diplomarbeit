<template>

    <div class="welcome">
        <h1 class="project__title">Willkommen im Kreis 3 von Zürich</h1>
        <div class="project__subtitle">
            <p>Eine Arbeit von Matthias Koch<br>Mentoriert von Richard Zimerman</p>
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
        margin-top: 5rem;
        margin-bottom: 5rem;
        color: #003041;
        font-family: "Suisse Neue";
    }

    .project__title {
        width: 100%;
    }

    .project__subtitle {
        width: 100%;
        font-size: 1.375rem;
        line-height: 2.0625rem;
    }

    .project__title {
        font-size: 5.125rem;
        line-height: 5.125rem;
        color: #003041;
        max-width: 43rem;
    }

    @media (max-width: 667px) {

        .project__title {
            font-size: 4.25rem;
            max-width: 100%;
            line-height: 4.25rem;
        }

        .project__subtitle {
            width: 100%;
        }
    }
</style>