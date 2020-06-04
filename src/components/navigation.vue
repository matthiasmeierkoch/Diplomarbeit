<template>
    <div class="navigation_wrapper">
        <div id="navbar">
            <header id="header">
                <!--            <div>
                                <g-link class="site_name" to="/">{{ $static.metadata.siteName }}</g-link>
                            </div>-->
                <nav class="nav">
                    <g-link class="nav__link" to="/"  exact>Über das Projekt</g-link>
                    <g-link class="nav__link" to="/about/">Kreis 3 App</g-link>
                </nav>
            </header>
        </div>
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


    export default {

        mounted() {
            let prevScrollpos = window.pageYOffset;
            window.onscroll = function () {
                let currentScrollPos = window.pageYOffset;
                if (prevScrollpos > currentScrollPos) {
                    document.getElementById("navbar").style.top = "0";
                } else {
                    document.getElementById("navbar").style.top = "-150px";
                }
                prevScrollpos = currentScrollPos;
            }
        }
    }
</script>

<style scoped>

    template {
        padding-left: 0;
        padding-right: 0;
    }

    #navbar {
        top: 0;
        left: 0;
        z-index: 100;
        transition: top 0.3s;
        display: flex;
        justify-content: space-between;
        position: fixed;
        width: 100%;
        height: 5rem;
        align-items: center;
        background-color: rgba(252, 251, 249, 1);
    }

    .nav {
        display: flex;
        justify-content: space-between;
        font-size: 1.25rem;
        font-weight: bold;
        margin: auto;
    }

    #header {
        margin: auto;
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
        justify-content: space-between;
        color: #003041;
        padding: 16px 24px;
        border-radius: 5rem;
        text-decoration: none;
        margin-right: 2rem;
        font-weight: bold;
    }

    .nav__link.active {
        color: #ffffff;
        background-color: #E4665C;
    }

    .nav__link:hover {
        color: #ffffff;
        background-color: rgba(228, 102, 92, 1);
    }

    .site_name:hover {
        color: #ffffff;
        background-color: #E4665C;
    }


    @media (max-width: 768px) {

        .site_name {
            padding: 8px 16px;
            margin-left: 2rem;
        }

        .site_name:hover {

        }

        #header {

        }

        .nav__link {
            font-size: 1.25rem;
        }

        .nav__link:hover {

        }

    }

    @media (max-width: 420px) {

        .site_name {
            padding: 8px 16px;
            margin-left: 0;
        }

        .site_name:hover {
            margin-left: 0;
        }

        #header {

        }

        .nav__link {
            font-size: 1rem;
            padding: 8px 16px;
        }

        .nav__link:hover {

        }

    }
</style>