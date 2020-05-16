<template>
    <div class="lead">
        <h2 class="lead__title">{{ title }}</h2>
        <div class="lead__content">
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
    .lead {
        position: relative;
        margin: auto;
        margin-top: 1.5rem;
        margin-bottom: 2rem;
        max-width: 75ch;
    }

    .lead__title {

    }

   .lead__content {
        color: #0066CC;
        font-size: 2rem;
        line-height: 3rem;
    }


    p {
        font-family: 'inter', sans-serif;
        color: #0066CC;

    }

    h3{
        font-family: 'inter', sans-serif;
        font-size: 1.325rem;
    }

    h2{
        font-family: 'inter', sans-serif;
        font-size: 2.5rem;
        color: #111111 ;
        -webkit-margin-before: 0.35em;
        margin-block-end: 0.35em;
    }

    @media (max-width: 667px) {

        .lead {
            display: contents;
            font-size: 2rem;
            line-height: 3rem;
        }

        .lead__title{
            width: 100%;
            margin-top: 3rem;
        }

        .lead__content{
            width: 100%;
            margin-top: 1rem;
            font-size: 1.825rem;
            line-height: 2.825rem;
            color: #0066CC;
        }
    }

</style>
