<!-- SCRIPT -->
<script setup>
    let text = '<p style="color:red">Testing v-html</p>';
</script>

<template>
    <div v-html="text"></div>
    <div>{{ text }}</div>
</template>
<!-- HTML -->