<template>
    <div class="row mb-3 align-items-center justify-content-center">
        <div class="col-12">
            <button class="btn" @click="$emit('mudarImagem')">Trocar Imagem</button>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MudarImagem',
    emits: ['mudarImagem']
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