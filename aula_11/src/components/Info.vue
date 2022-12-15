<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento!</p>
        <p v-else>Estou em busca de novas oportunidades!</p>
        <p v-show="esta_trabalhando">Utilizio as seguintes tecnologias:</p>
        <ul v-show="esta_trabalhando">
            <li>Html5</li>
            <li>CSS3</li>
            <li>JS</li>
            <li>Vue</li>
        </ul>
        
        <Picture />

        <div class="text-center">
            <button @click="ShowEmail" class="btn">{{text_botao}}</button>
        </div>

        <p v-show="mostrar_email">Mande uma mensagem para: {{email}}</p>
        
        <p>Para acessar meu portifólio <strong><a v-bind:href="meu_link" target="_blank">basta clicar aqui</a></strong>!</p>
    </div>
</template>

<script>

import Picture from './Picture.vue';

export default {
    name: 'info',
    components: {
    Picture
  },
    data(){
        return{
            esta_trabalhando: false,
            mostrar_email: false,
            email: 'janaina.adolfo.ds@gmail.com',
            meu_link: 'https://github.com/Jana-SI',
            text_botao: 'Mostar E-mail'
        }
    },
    methods: {
        ShowEmail(){
            this.mostrar_email = !this.mostrar_email

            if(!this.mostrar_email){
                this.text_botao = 'Mostrar E-mail'
            }else{
                this.text_botao = 'Esconder E-mail'
            }
        }
    }
}
</script>

<style>
a{ color: #37495f !important;}
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