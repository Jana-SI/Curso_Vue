<template>
  <div class="container-fluid">
    <div id="rowP" class="row align-items-center justify-content-center">
      <div class="col-6 col-sm-6 col-md-6 col-lg-6">
        <div class="card text-bg-success border border-white">
          <div class="card-header text-center border-bottom border-white">
            <h2><strong>Curso Vue</strong></h2>
          </div>
          <div class="card-body">
            <h3 class="card-title text-center "><strong>Aula 15</strong></h3>
            <Multiplos_Eventos />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

import Multiplos_Eventos from './components/Multiplos_Eventos.vue';

export default {
  name: "App",
  components: {
    Multiplos_Eventos
  }
};
</script>

<style>
body {
  background-image: url(./assets/fundo.jpg);
}

#rowP {
    height: 100vh;
}

h2,
h3 {
  color: #37495f !important;
}

.card-text {
  padding: 5px;
}
</style>