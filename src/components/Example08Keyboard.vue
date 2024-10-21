<!-- SCRIPT -->

<script setup>
    function message(){
        alert('Running the function');
    }
</script>

<!-- HTML -->

<template>
    <input type="text" @keyup.enter="message">
</template>