<template>

  <div class="container-fluid">
    <div class="row align-items-center justify-content-center">
      <div class="col-6 col-sm-6 col-md-6 col-lg-6 text-center">
        <div class="card text-bg-success text-center border border-white">
          <div class="card-header border-bottom border-white">
            <h2><strong>Curso Vue</strong></h2>
          </div>
          <div class="card-body">
            <h3 class="card-title"><strong>Aula 05</strong></h3>
            <h4 class="card-text border-top border-white">Olá mundo!</h4>
            <Primeiro_Componente />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Primeiro_Componente from './components/Primeiro_Componente.vue';

export default {
  name: "App",
  components: {
    Primeiro_Componente
  }
};
</script>

<style>
body {
  background-image: url(./assets/fundo.jpg);
}

.row {
  height: 100vh;
}

h2,
h3 {
  color: #37495f !important;
}
</style>