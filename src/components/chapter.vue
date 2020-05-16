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
        margin-top: 5rem;
        margin-bottom: 2rem;
    }

    .chapter__title {
        width: 100%;
    }

    .chapter__content {
        width: 100%;
        font-size: 1.3rem;
        line-height: 1.8rem;
    }


    p {
        font-family: 'inter', sans-serif;
        color: #111111 ;
    }

    h3{
        font-family: 'inter', sans-serif;
        font-size: 1.325rem;
    }

    h2{
        font-family: 'inter', sans-serif;
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
