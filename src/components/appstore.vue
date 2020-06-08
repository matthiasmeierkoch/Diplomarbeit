<template>
    <div class="container">
        <div class="content">
            <p>Lade dir jetzt die App herunter und wird zum Teil des Kreis 3</p>
        </div>
        <div class="appbilder">
            <g-image src="../assets/img/appstore.png"></g-image>
        </div>
    </div>
</template>

<script>
    export default {
        name: "appstore"
    }
</script>

<style scoped>
    .container {
        background-color: #FCFBF9;
        color: #003041;
        border-radius: 1rem;
        width: 100%;
        margin-bottom: 5rem;
        padding: 2rem;
        font-family: "Suisse Neue";
    }

    .content {
        font-size: 2.25rem;
        width: 100%;
        text-align: center;
    }

    .appbilder {
        width: 35%;
        margin: auto;
    }

    p{
        font-family: "Suisse Neue";
        font-size: 3rem;
    }

    @media (max-width: 780px) {
        .container {
            display: block;
            width: auto;
            margin-top: 3rem;
            padding: 1rem;
        }

        .content {
            text-align: center;
            font-size: 1.8rem;
            font-weight: bold;
        }

        .appbilder {
            margin: auto;
            width: 70%;
        }
        p{
            font-size: 2rem;
        }

    }

</style>