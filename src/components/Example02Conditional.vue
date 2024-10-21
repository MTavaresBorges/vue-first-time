<!-- SCRIPT -->

<script setup>
    let show = true;
    let media = 6.5;
</script>

<!-- HTML -->

<template>
    <h1 v-if="show">Hello World!</h1>

    <p v-if="media >= 7">Approved</p>
    <p v-else-if="media >= 5">Pending</p>
    <p v-else=>Reproved</p>
</template>