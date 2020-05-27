<template>
    <div class="weekday">
    <p class="">Happy {{ weekday }} !</p>
    </div>

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
        font-size: 1.5rem;
        margin-top: 4rem;
        text-align: center;
    }
</style>