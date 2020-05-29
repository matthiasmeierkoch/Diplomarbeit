<template>
    <div id="navbar">
        <header id="header">
            <div>
                <g-link class="site_name" to="/">{{ $static.metadata.siteName }}</g-link>
            </div>
            <nav class="nav">
                <g-link class="nav__link" to="/">Über das Projekt</g-link>
                <g-link class="nav__link" to="/about/">Kreis 3 App</g-link>
            </nav>
        </header>
    </div>
</template>

<static-query>
    query {
    metadata {
    siteName
    }
    }
</static-query>

<script>
    /*    let prevScrollpos = window.pageYOffset;
        window.onscroll = function () {
            let currentScrollPos = window.pageYOffset;
            if (prevScrollpos > currentScrollPos) {
                document.getElementById("navbar").style.top = "0";
            } else {
                document.getElementById("navbar").style.top = "-80px";
            }
            prevScrollpos = currentScrollPos;
        }*/
</script>

<style>

    #navbar {
        top: 0;
        z-index: 100;
    }

    .nav {
        right: 0;
    }

    #header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 20px;
        font-size: 1.25rem;
        font-weight: bold;
        position: relative;
        transition: top 0.3s;
        padding-top: 24px;
        padding-bottom: 24px;
        border-radius: 100px;

    }

    .site_name {
        display: flex;
        margin-left: 2rem;
        color: #E4665C;
        padding: 16px 24px;
        border-radius: 5rem;
        background-color: #ffffff;
        text-decoration: none;

    }

    .nav__link {
        margin-left: 2rem;
        color: #E4665C;
        padding: 16px 24px;
        border-radius: 5rem;
        background-color: #ffffff;
        text-decoration: none;
    }

    .nav__link:hover {
        margin-left: 2rem;
        color: #ffffff;
        background-color: #E4665C;
    }

    .site_name:hover {
        margin-left: 2rem;
        color: #ffffff;
        background-color: #E4665C;
    }

    @media (max-width: 667px) {

        #header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
            height: 80px;
            font-size: 1rem;
            font-weight: bold;
            width: 100vw;
        }

        .nav__link {
            margin-left: 1rem;
            color: #ffffff;
            text-decoration: none;
        }

        .nav__link:hover {
            margin-left: 1rem;
            color: #E4665C;
            border-bottom: 4px solid #E4665C;
            stroke-linecap: round;
        }

    }
</style>