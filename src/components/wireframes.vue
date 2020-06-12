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
        margin-left: 3rem;
        transform: scale(1.0);
        -o-transition: 02s ease-out;
        -ms-transition: 0.2s ease-out;
        -moz-transition: 0.2s ease-out;
        -webkit-transition: 0.2s ease-out;
    }

    .thumbnail :hover{
        transform: scale(1.2);
        -o-transition: 02s ease-out;
        -ms-transition: 0.2s ease-out;
        -moz-transition: 0.2s ease-out;
        -webkit-transition: 0.2s ease-out;
    }


</style>