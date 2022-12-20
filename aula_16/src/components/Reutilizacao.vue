<template>
    <div class="row mb-3 align-items-center justify-content-center">
        <div class="col-6 text-center">
            <button class="btn" @click="ativar">clique aqui</button>
        </div>
        <div class="col-6 text-center">
            <p v-show="ativou">Ativado!</p>
        </div>
    </div>
</template>

<script>
export default{
    name: 'Reutilizacao',
    data(){
        return{
            ativou: false
        }
    },
    methods: {
        ativar(){
            this.ativou = !this.ativou
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