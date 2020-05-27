<template>
    <div class="content" data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
         data-sal-easing="ease-out-bounce">
        <div class="Section">
            <div class="Section__image">
                <div data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
                     data-sal-easing="ease-out-bounce">
                    <g-image calss="Section__image" width="400" src="../assets/img/Startseite.png"></g-image>
                </div>
            </div>
            <div class="Section__content">
                <h2 class="Section__title">{{ title }}</h2>
                <slot></slot>
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

<style>


    .Section {
        position: relative;
        display: flex;
        justify-content: space-between;
        align-items: center;
        max-width: 100%;
        margin-top: 7rem;
    }

    .Section__image {
        max-width: 50%;
        margin: auto;
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

    @media (max-width: 667px) {

        .Section {
            display: contents;
        }

        .Section__title {
            width: 100%;
            font-size: 3.5rem;
            margin-top: 4rem;

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
            margin-top: 4rem;

        }

        .Section__content {
            max-width: 100%;
            margin-top: 2rem;
        }
    }

</style>
