<template>
    <img class="rounded rounded mx-auto d-block" :src="avatar" :alt="descricao">
    <MudarImagem @mudar-imagem="trocarImagem" @click="voltarImagem()"/>
</template>

<script>
import MudarImagem from './MudarImagem.vue';

export default {
    name: "Picture",
    components: { 
        MudarImagem 
    },
    data() {
        return {
            avatar: "/img/avatar.png",
            descricao: "img de avatar"
        };
    },
    methods: {
        trocarImagem(){
            this.avatar="/img/avatar2.png"
        },
        voltarImagem() {
           setTimeout(() => {
            this.avatar="/img/avatar.png"
           }, 2000);
           
        }
    }
}
</script>