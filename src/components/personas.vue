<template>
    <div class="persona">
        <div class="persona__content">
            <LightBox class="thumbnail" :thumbnail="images[0]" :images="images"/>
        </div>
    </div>
</template>

<script>
    import LightBox from "./LightBox";

    export default {
        name: "personas",
        components: {
            LightBox
        },

        data() {
            return {
                images: ["/Persona - Jan Neumann.png", "Persona - Lara Schreiber.png", "Persona - Larissa Spirituell.png", "Persona - Valentin Christen.png"]
            }
        },

    }
</script>

<style scoped>

    .persona {
        display: flex;
        justify-content: space-between;
    }


    .thumbnail {
        width: 100%;
    }

</style>