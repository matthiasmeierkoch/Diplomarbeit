<template>

    <p class="weekday">Happy {{ weekday }} !</p>

</template>

<script>
    const dayName = ['Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday'];
    let day = new Date().getDay();
    let weekdayName = dayName[day];

    export default {
        data() {
            return { weekday: weekdayName}
        }
    }
</script>


<style>
    .weekday{
        font-family: "Suisse BP Int";
        font-size: 1.25rem;
        margin: 1rem, auto;
    }
</style>