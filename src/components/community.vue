<template>
    <div class="content">
        <div class="Section" data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
             data-sal-easing="ease-out-bounce">
            <div class="Section__content">
                <h2 class="Section__title">{{ title }}</h2>
                <slot></slot>
            </div>
            <div class="Section__image">
                <div data-sal="slide-up"
                     data-sal-delay="100"
                     data-sal-duration="1000"
                     data-sal-easing="ease-out-bounce">
                    <g-image calss="Section__image" width="400" src="/community.jpg"></g-image>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    import sal from 'sal.js';

    export default {
        props: ['title'],
        mounted() {
            this.$nextTick(() => sal());
        }
    }
</script>

<style scoped>

    .Section {
        position: relative;
        display: flex;
        justify-content: space-between;
        align-items: center;
        max-width: 100%;
        margin-top: 2.5rem;
        height: 90vh;
    }

    .Section__image {
        max-width: 50%;
        margin: auto;
        display: flex;
        justify-content: center;
    }

    .Section__image img {
        width: 800px;
        z-index: -5;
        border-radius: 1rem ;
    }


    .Section__title {
        width: 100%;
        font-size: 4rem;
        line-height: 5.5rem;
        color: #003041;
        font-family: "Suisse Neue";
        text-align: center;
    }

    .Section__content {
        max-width: 50%;
        font-size: 2rem;
        line-height: 3rem;
        color: #003041;
        margin: auto;
        font-family: "Suisse Neue";
        text-align: left;
        background-color: #FCFBF9;
        border-radius: 1rem;
        padding: 2rem;
        z-index: 1;
    }

    h2 {
        font-size: 2rem;
    }

    p{
        margin-top: 1rem;
    }


    @media (max-width: 520px) {
        .Section__image img {
            margin-top: -2.5rem;
            display: block;
            width: 100%;
        }

        .Section__title {
            width: 100%;
            font-size: 2rem;
            line-height: 3.25rem;
            margin-top: 6rem;

        }
    }

    @media (max-width: 768px) {

    }

    @media (max-width: 900px) {

        .content{
        }

        .Section {
        }

        .Section__title {
            max-width: 100%;
            font-size: 3.5rem;
            line-height: 4.25rem;
            margin-top: 1rem;
            text-align: center;
        }

        .Section__content {
            max-width: 100%;
            margin-top: 5rem;
            font-size: 2rem;
            line-height: 3.5rem;
            padding:2rem;
            text-align: center;
        }
    }

</style>
