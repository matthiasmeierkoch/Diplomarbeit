<template>
    <div class="background">
        <div>
            <!--<g-image class="background__image" src="../assets/img/zurich.jpg"/>-->
            <div class="gradient"></div>
            <video autoplay loop muted class="background__image" src="../assets/img/video.mp4"></video>
        </div>
    </div>
</template>

<script>
    export default {
        name: "background"
    }
</script>

<style scoped>

    .background__image {
        position: absolute;
        z-index: -10;
        width: 100%;
        height: 100vh;
        top: 0;
        left: 0;
        object-fit: cover;
    }


    .gradient{
        position: absolute;
        top:0;
        left:0;
        background-image: linear-gradient(to bottom, rgba(0,0,0,0), rgba(0,0,0,1));
        width: 100%;
        height: 100vh;
        opacity: 0.7;
        z-index: -9;

    }


    .background {
    }

</style>