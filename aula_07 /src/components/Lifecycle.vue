<template>
    <p class="card-text border-top border-white">Meu nome é: {{nome}}</p>
</template>

<script>
export default{
    name: 'Lifecycle',
    data(){
        return{
            nome: 'Ainda não informado!'
        }
    },
    created(){
        setTimeout(() => {
            this.nome = "Janaina"
        }, 1000);
    },
    mounted(){
        setTimeout(() => {
            this.nome = "Carlos"
        }, 2000);
    }
}
</script>