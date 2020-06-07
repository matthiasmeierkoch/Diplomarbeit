<template>
    <div class="quote">
        <div class="quote__content">
            <slot></slot>
        </div>
        <p class="quote__autor">{{ title }}</p>
    </div>
</template>

<script>
    export default {
        name: "Quote",
        props: ['title']
    }
</script>

<style scoped>
    .quote {
        background: #FCFBF9;
        padding: 1.8rem;
        border-radius: 1.5rem;
        width: 70%;
        margin: auto;
        margin-bottom: 5rem;
        margin-top: 5rem;
    }

    .quote__autor {
        font-size: 1rem;
        padding-left: 1.5rem;
    }

    .quote__content {
        font-size: 1.75rem;
        line-height: 2.5rem;
        font-weight: bold;
        padding-left: 1.5rem;
        padding-right: 1.5rem;
    }

    @media (max-width: 768px) {

        .quote {
            width: 100%;
            padding: 0;
        }
        .quote__autor{
            padding-left: 1rem;
            padding-bottom: 1.5rem;
        }
        .quote__content{
            font-size: 1.5rem;
            line-height: 2.25rem;
            padding-left: 1rem;
            padding-top: 0.25rem;
        }

    }

</style>