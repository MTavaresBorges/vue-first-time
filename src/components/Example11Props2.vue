<!-- SCRIPT -->
<script setup>

    const props = defineProps(['name', 'age']);

</script>

<!-- HTML -->
<template>
    <h1>Name: {{ name }}</h1>
    <h2>Age: {{ age }}</h2>
</template>