<template>

  <div class="container-fluid">
    <div class="row align-items-center justify-content-center">
      <div class="col-6 col-sm-6 col-md-6 col-lg-6">
        <div class="card text-bg-success border border-white">
          <div class="card-header text-center border-bottom border-white">
            <h2><strong>Curso Vue</strong></h2>
          </div>
          <div class="card-body">
            <h3 class="card-title text-center "><strong>Aula 09</strong></h3>
            <Pessoa />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

import Pessoa from './components/Pessoa.vue';

export default {
  name: "App",
  components: {
    Pessoa
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

.card-text{
  padding: 5px;
}
</style>