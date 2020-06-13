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
        </div>
    </div>
</template>

<script>
    import LightBox from "./LightBox";

    export default {
        name: "concept",
        components: {
            LightBox
        },

        data() {
            return {
                images: ["/Onboarding.png", "/Entdecken.png", "/Bucketlists.png"]
            }
        },

    }
</script>

<style scoped>

    .persona {
        display: block;
        justify-content: space-between;
    }

    .persona__content{
        display:block;
    }
    .thumbnail {
        width: 100%;
        margin-left: 1rem;
        margin-top: 2rem;

    }

    .thumbnail :hover {
        box-shadow: 0 20px 40px -20px rgba(0, 0, 0, 0.3);
    }

</style>