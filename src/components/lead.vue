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
        margin: 28vh auto 2rem;
        max-width: 65ch;
    }

    .lead__title {

    }

    .lead__content {
        color: #003041;
        font-size: 2rem;
        line-height: 3rem;
        font-family: "Suisse Neue";
    }

    h3{
        font-family: 'Suisse Neue', sans-serif;
        font-size: 1.5rem;
        line-height: 2.25rem;
    }

    h2{
        font-family: 'Suisse Neue', sans-serif;
        font-size: 2.5rem;
        color: #003041 ;
        -webkit-margin-before: 0.35em;
        margin-block-end: 0.35em;
    }


    @media (max-width: 768px) {

        .lead {
            display: contents;
            font-size: 2rem;
            line-height: 3rem;
            margin-top: 2rem;
        }

        .lead__title{
            width: 100%;
            margin-top:30rem;
        }

        .lead__content{
            width: 100%;
            margin-top: 1rem;
            font-size: 1.825rem;
            line-height: 2.825rem;
            color: #0066CC;
        }
    }

@media (max-width: 420px) {
    .lead__title{
        width: 100%;
        margin-top: 16rem;
    }
}


</style>
