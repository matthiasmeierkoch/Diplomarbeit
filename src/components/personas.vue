<template>
    <div class="persona">
        <div class="persona__content">
            <LightBox data-sal="slide-up"
                      data-sal-delay="100"
                      data-sal-duration="1000"
                      data-sal-easing="ease-out-bounce"
                      class="thumbnail" :thumbnail="images[0]" :images="images"/>
            <LightBox data-sal="slide-up"
                      data-sal-delay="100"
                      data-sal-duration="1000"
                      data-sal-easing="ease-out-bounce"
                      class="thumbnail" :thumbnail="images[1]" :images="images"/>
            <LightBox data-sal="slide-up"
                      data-sal-delay="100"
                      data-sal-duration="1000"
                      data-sal-easing="ease-out-bounce"
                      class="thumbnail" :thumbnail="images[2]" :images="images"/>
            <LightBox data-sal="slide-up"
                      data-sal-delay="100"
                      data-sal-duration="1000"
                      data-sal-easing="ease-out-bounce"
                      class="thumbnail" :thumbnail="images[3]" :images="images"/>
            <LightBox data-sal="slide-up"
                      data-sal-delay="100"
                      data-sal-duration="1000"
                      data-sal-easing="ease-out-bounce"
                      class="thumbnail" :thumbnail="images[4]" :images="images"/>
        </div>
    </div>
</template>

<script>
    import LightBox from "./LightBox";
    import sal from "sal.js";

    export default {
        name: "personas",
        components: {
            LightBox
        },

        data() {
            return {
                images: ["/Persona - Jan Neumann.png", "/Persona - Lara Schreiber.png", "/Persona - Larissa Spirituell.png", "/Persona - Valentin Christen.png", "/Benutzerrollen.png"]
            }
        },

        mounted() {
            this.$nextTick(() => sal());
        }

    }
</script>

<style scoped>

    .persona {
        width: 100%;
    }

    .persona__content {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
    }

    .thumbnail {
        width: 46.5%;
        margin-left: 1rem;
        margin-top: 2rem;
        -o-transition: 02s ease-out;
        -ms-transition: 0.2s ease-out;
        -moz-transition: 0.2s ease-out;
        -webkit-transition: 0.2s ease-out;
    }

    .thumbnail :hover {
        transform: scale(1.1);
        -o-transition: 02s ease-out;
        -ms-transition: 0.2s ease-out;
        -moz-transition: 0.2s ease-out;
        -webkit-transition: 0.2s ease-out;
    }

    @media (max-width: 520px) {
        .thumbnail {
            width: 100%;
        }

    }

</style>