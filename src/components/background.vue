<template>
    <div class="background">
        <div>
            <g-image class="background__image" src="../assets/img/zurich.jpg"/>
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
        height: 100%;
        top: 0;
        left: 0;
        object-fit: cover;
    }

    .background {
        width: 100vw;
    }

</style>