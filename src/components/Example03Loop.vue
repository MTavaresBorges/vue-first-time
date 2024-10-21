<!-- SCRIPT -->

<script setup>
    let cars = ['Subaru Impreza WRX - 1996', 'Chevrolet Corvette C4 - 1991', 'Nissan Skyline R32 GTR - 1994', 'Mitsubishi GTO - 1998', 'Nissan 240SX - 1996'];
</script>

<!-- HTML -->

<template>
    <h3>Positions:</h3>
    <ul>
        <li v-for="car in cars">{{ car }}</li>
    </ul>
</template>