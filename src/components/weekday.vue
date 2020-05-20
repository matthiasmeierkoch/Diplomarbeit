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
        margin: 0, auto;
    }
</style>