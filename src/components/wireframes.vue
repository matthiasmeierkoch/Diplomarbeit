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
                images: ["/Userjourney.png", "/Wireframes.png"]
            }
        },

    }
</script>

<style scoped>

    .persona {
        display: flex;
        justify-content: space-between;
    }

    .persona__content{
        display:flex;
    }
    .thumbnail {
        width: 50%;
        margin-left: 1rem;
    }
</style>