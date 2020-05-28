<template>
    <div class="chapter">
        <h2 class="chapter__title">{{ title }}</h2>
        <div class="chapter__content">
            <slot></slot>
        </div>
    </div>
</template>

<script>
    export default {
        props: ['title']
    }
</script>

<style>
    .chapter {
        position: relative;
        margin: 5rem auto 2rem;
        max-width: 65ch;
    }

    .chapter__title {
        width: 100%;
        margin-top: 4rem;
    }

    .chapter__content {
        width: 100%;
        font-size: 1.375rem;
        line-height: 2.0625rem;
    }


    p {
        font-family: 'Suisse BP Int', sans-serif;
        color: #003041 ;
    }

    h3{
        font-family: 'Suisse Neue', sans-serif;
        font-size: 1.5rem;
        line-height: 2.25rem;
    }

    h2{
        font-family: 'Suisse BP Int', sans-serif;
        font-size: 3.5rem;
        line-height: 4rem;
        color: #0066CC;
        -webkit-margin-before: 0.35em;
        margin-block-end: 0.35em;
    }

    @media (max-width: 667px) {

        .chapter {
            display: contents;
        }

        .chapter__title{
            width: 100%;
            margin-top: 3rem;
        }

        .chapter__content{
            width: 100%;
            margin-top: 1rem;
        }
    }

</style>
