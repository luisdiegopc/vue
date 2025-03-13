<template>
<h1 v-if="exibir">Olá, tudo OK!</h1>

<p v-if="media >= 7">Aprovado(a)</p>
<p v-else-if="media >= 5">Em exame</p>
<p v-else>Reprovado(a)</p>

</template>

<script>
let exibir = false
let media = 9

export default {
  name: "Ex2condicional",
};
</script>