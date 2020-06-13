<template>
    <div class="persona">
        <div class="persona__content">
            <LightBox class="thumbnail" :thumbnail="images[0]" :images="images"/>
            <LightBox class="thumbnail" :thumbnail="images[1]" :images="images"/>
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
                images: ["/Atoms.png", "/Components.png"]
            }
        },

    }
</script>

<style scoped>

    .persona {
        display: flex;
        justify-content: space-between;
        margin-top: 3rem;
    }

    .persona__content{
        display:flex;
    }
    .thumbnail {
        width: 50%;
        margin-left:3rem;

    }

    .thumbnail :hover{
        box-shadow: 0 20px 40px -20px rgba(0, 0, 0, 0.3);
    }

</style>