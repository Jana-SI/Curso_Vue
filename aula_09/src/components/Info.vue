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
        <p v-show="mostrar_email">Mande uma mensagem para: {{email}}</p>
    </div>
</template>

<script>
export default {
    name: 'info',
    data(){
        return{
            esta_trabalhando: false,
            mostrar_email: true,
            email: 'janaina.adolfo.ds@gmail.com'
        }
    }
}
</script>