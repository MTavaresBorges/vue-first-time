<!-- SCRIPT -->
<script setup>

    import { onMounted, ref } from 'vue';

    let text = ref('Hello World!');

    onMounted(() => {
        setTimeout(() => {
            text.value = "Changing text";
        }, 3000);
    });
</script>

<!-- HTML -->

<template>
    <h1>{{ text }}</h1>
</template>