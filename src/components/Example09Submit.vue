<!-- SCRIPT -->
<script setup>

    function validatesForm(event){
        alert('Form sent');

        event.preventDefault();
    }

</script>
<!-- HTML -->

<template>

    <form action="https://www.google.com.br/?hl=pt-BR" @submit="validatesForm">
        <input type="submit" value="Send Form">
    </form>

</template>