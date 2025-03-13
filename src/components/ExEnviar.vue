<script setup>
function validaForm(event) {
    alert('Formulário enviado!')
    event.preventDefault()
 }
</script>

<template>

<form action="http://globo.com" @submit="validaForm">
    <input type="submit" value="Enviar Formulário">    
</form>
</template>