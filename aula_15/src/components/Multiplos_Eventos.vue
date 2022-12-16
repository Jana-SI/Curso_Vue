<template>
    <div class="row mb-3 align-items-center justify-content-center">
        <div class="col-6">
            <button class="btn" @click="primeiro(txt1, $event), segundo(txt2, $event), terceiro()">Ativar Múltiplos Eventos</button>
        </div>
        <div class="col-12 text-center">
            <p>{{ mult_eventos }}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Multiplos_Eventos',
    data() {
        return {
            mult_eventos: "",
            txt1: "Primeiro evento ativado!",
            txt2: "Segundo evento ativado!"
        }
    },
    methods: {
        primeiro(txt, e) {
            e.preventDefault();
            this.mult_eventos = txt;
        },
        segundo(txt, e) {
            e.preventDefault();
           setTimeout(() => {
            this.mult_eventos = txt;
           }, 1000);
        },
        terceiro() {
           setTimeout(() => {
            this.mult_eventos = "";
           }, 2000);
           
        }
    }
}
</script>

<style scoped>
.btn {
    background-color: #37495f !important;
    color: white !important;
    border: 2px solid white;
}

.btn:hover {
    background-color: white !important;
    color: #37495f !important;
    border: 2px solid #37495f !important;
}
</style>