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
        background: #FFDBBB;
        padding: 1.8rem;
        border-radius: 1.5rem;
        width: 80%;
        margin: auto;
    }

    .quote__autor {
        font-size: 1.75rem;

    }

    .quote__content {
        font-size: 1.75rem;
        line-height: 2.5rem;
        font-weight: bold;
    }
</style>