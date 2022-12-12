<template>
  <div class="card-text border-top border-white">
    <p>Nome: {{ nome }}</p>
    <p>Idade: {{ idade }}</p>
    <p>Profissão: {{ profissao }}</p>
  </div>
</template>

<script>
export default {
  name: 'PrimeiroComponente',
  data() {
    return {
      nome: "Janaina",
      idade: 29,
      profissao: "Front-End"
    }
  }
}
</script>