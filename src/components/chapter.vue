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
        justify-content: space-between;
        display: flex;
        padding-top: 3rem;
    }

    .chapter__title {
        width: 50%;
    }

    .chapter__content {
        width: 50%;
    }


    p {
        font-family: 'inter', sans-serif;
        font-size: 1.125rem;
        color: #0070BC ;
    }

    h3{
        font-family: 'inter', sans-serif;
        font-size: 1.325rem;
    }

    h2{
        font-family: 'inter', sans-serif;
        font-size: 2.5rem;
        color: #0070BC ;
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
