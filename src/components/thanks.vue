<template>
    <div class="thanks">
        <h2 class="chapter__title">{{ title }}</h2>
        <div data-sal="slide-up"
             data-sal-delay="100"
             data-sal-duration="1000"
             data-sal-easing="ease-out-bounce">
            <h3>Diplomarbeitarbeit von:</h3>
            <p>Matthias Koch</p>
        </div>
        <div data-sal="slide-up"
             data-sal-delay="100"
             data-sal-duration="1000"
             data-sal-easing="ease-out-bounce">
            <h3>Mentoriert von:</h3>
            <p>Richard Zimerman<br>
                <a href="https://www.zcreativelabs.com/" target="_blank">z creative labs</a>
            </p>
        </div>

        <div data-sal="slide-up"
             data-sal-delay="100"
             data-sal-duration="1000"
             data-sal-easing="ease-out-bounce">
            <h3>Bildungsgang:</h3>
            <p>Dipl. Gestalter/-in HF Fachrichtung Kommunikationsdesign mit Vertiefungsrichtung Interaction Design<br>
                <a href="https://sfgz.ch/" target="_blank">Schule für Gestaltung Zürich</a>
            </p>
        </div>
        <div data-sal="slide-up"
             data-sal-delay="100"
             data-sal-duration="1000"
             data-sal-easing="ease-out-bounce">
            <h3>Bilder von:</h3>
            <p><a href="https://unsplash.com" target="_blank">Unsplash</a></p>
        </div>
    </div>
</template>

<script>
    import sal from "sal.js";

    export default {
        name: "thanks",
        props: ['title'],

        mounted() {
            this.$nextTick(() => sal());
        }
    }



</script>

<style scoped>
    .thanks {
        display: block;
        justify-content: space-between;
    }

    .mentor__name {
        max-width: 50%;
        margin-left: 1rem;
    }

    .autor__name {
        max-width: 50%;
        margin-left: 1rem;
    }

    h3 {
        color: #003041;
        font-size: 1.325rem;
        margin-bottom: -1rem;
        margin-top: 2.5rem;
    }

    p {
        font-size: 1.325rem;
    }

    @media (max-width: 780px) {
        .thanks {
            display: block;
        }

        .mentor__name {
            max-width: 100%;
            margin-left: 0;
        }

        .autor__name {
            max-width: 100%;
            margin-left: 0;
        }
    }

</style>