<template>
    <div class="background">
        <div>
            <g-image class="background__image" src="../assets/img/Background.png"/>
        </div>
    </div>
</template>

<script>
    export default {
        name: "aboutbackground"
    }
</script>

<style scoped>

    .background__image {
        position: absolute;
        z-index: -10;
        width: 100vw;
        top: 0;
        left: 0;

    }

    .background {
        background: linear-gradient(90deg, rgba(0,0,0,1) 0%, rgba(255,255,255,0) 50%);
    }

    @media (max-width: 900px) {

        .background__image {
            position: fixed;
        }
    }
</style>