<!-- SCRIPT -->

<script setup>
    let validation = false;
</script>

<!-- CSS -->
<style>
    .success{color: green}

    .fail{color: red}
</style>

<!-- HTML -->

<template>
    <p :class="validation ? 'success' : 'fail'">Using class</p>
</template>