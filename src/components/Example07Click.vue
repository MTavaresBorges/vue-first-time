<!-- SCRIPT -->

<script setup>

    function message(){
        alert('Testing clicking events');
    }

</script>

<!-- HTML -->

<template>
    <button @click="message">Click here</button>
</template>