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
                    <g-image calss="Section__image" width="400" src="../assets/img/Startseite_Transparent.gif"></g-image>
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

    .background__image{
        position: absolute;
        z-index: -10;
        width: 100%;
        height: 100vh;
        top: 0;
        left: 0;
        object-fit: cover;
    }

    .Section {
        position: relative;
        display: flex;
        justify-content: space-between;
        align-items: center;
        max-width: 100%;
        margin-top: 2.5rem;
        height: 100vh;
    }

    .Section__image {
        max-width: 50%;
        margin: auto;
        display: flex;
        justify-content: center;
    }

    .Section__image img {
        width: 320px;
    }


    .Section__title {
        width: 100%;
        font-size: 5rem;
        line-height: 6rem;
        color: #003041;
        font-family: "Suisse Neue";
        text-align: center;
    }

    .Section__content {
        max-width: 50%;
        font-size: 2rem;
        line-height: 3rem;
        color: #003041;
        margin-top: -3rem;
        font-family: "Suisse Neue";
        text-align: center;
    }

    @media (max-width: 420px) {
        .Section__image img {
            margin-top: 1rem;
        }

        .Section__title {
            width: 100%;
            font-size: 3rem;
            line-height: 4rem;
            margin-top: 6rem;

        }
    }

    @media (max-width: 768px) {

        .Section {
            display: contents;
            margin-top: 5rem;
        }

        .Section__title {
            width: 100%;
            font-size: 3.5rem;
            margin-top: 6rem;

        }

        .Section__content {
            max-width: 100%;
            margin-top: 2rem;
        }
    }

    @media (max-width: 900px) {

        .Section {
            display: contents;
        }

        .Section__title {
            max-width: 100%;
            font-size: 3.5rem;
            line-height: 4.25rem;
            margin-top: 8rem;

        }

        .Section__content {
            max-width: 100%;
            margin-top: 2rem;
        }
    }

</style>
