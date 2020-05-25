<template>

    <div class="layout">
        <header class="header">
            <div>
                <g-link class="site_name" to="/">{{ $static.metadata.siteName }}</g-link>
            </div>
            <nav class="nav">
                <g-link class="nav__link" to="/">Über das Projekt</g-link>
                <g-link class="nav__link" to="/about/">Kreis 3 App</g-link>
            </nav>
        </header>
        <slot/>

    </div>

</template>

<static-query>
    query {
    metadata {
    siteName
    }
    }
</static-query>

<style>
    @font-face {
        font-family: "Suisse Neue";
        src: url(../assets/font/SuisseNeue-Regular-WebS.woff);
    }

    @font-face {
        font-family: "Suisse BP Int";
        src: url(../assets/font/SuisseIntl-Regular-WebS.woff);
    }

    body {
        font-family: "Suisse BP Int", system-ui, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
        margin: 0;
        padding: 0;
        line-height: 1.5;
        background: #FCFBF9;
    }

    .layout {
        max-width: 1110px;
        margin: 0 auto;
        padding-left: 20px;
        padding-right: 20px;
    }

    .header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 20px;
        height: 80px;
        font-size: 1.25rem;
        font-weight: bold;
    }

    .site_name {
        display: flex;
        width: 100%;
        color: #E4665C;
        text-decoration: none;
    }

    .nav__link {
        margin-left: 2rem;
        color: #E4665C;
    }
</style>
