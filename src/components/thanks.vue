<template>
    <div class="thanks">
        <h2 class="chapter__title" >{{ title }}</h2>
        <h3>Diplomarbeitarbeit von:</h3>
        <p>Matthias Koch</p>
        <h3>Mentoriert von:</h3>
        <p>Richard Zimerman<br>
            <a href="https://www.zcreativelabs.com/">z creative labs</a>
        </p>

        <h3>Bildungsgang:</h3>
        <p>Dipl. Gestalter/-in HF Fachrichtung Kommunikationsdesign mit Vertiefungsrichtung Interaction Design<br>
            <a href="https://sfgz.ch/">Schule für Gestaltung Zürich</a>
        </p>

        <h3>Bilder von:</h3>
        <p><a href="https://unsplash.com">Unsplash</a></p>

    </div>
</template>

<script>
    export default {
        name: "thanks",
        props: ['title']
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