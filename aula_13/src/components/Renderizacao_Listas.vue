<template>
    <p>Tecnologias Back-End:</p>
    <ul>
        <li v-for="(tecnologia, index) in backend_tecnologias" v-bind:key="index">{{ tecnologia }}</li>
    </ul>
    <p>Tecnologias Front-End:</p>
    <ul>
        <li v-for="tecnologia in frontend_tecnologias" v-bind:key="tecnologia.id">{{ tecnologia.language }}</li>
    </ul>
</template>
<script>
export default {
    name: 'Renderizacao_Listas',
    data() {
        return {
            backend_tecnologias: ['JS', 'PHP 8', 'Python'],
            frontend_tecnologias: [
                { id: 1, language: 'HTML5' },
                { id: 2, language: 'CSS3' },
                { id: 3, language: 'Vue 3' },
            ]
        }
    }
}
</script>

<style scoped>
ul {
    list-style: none;
    display: flex;
    justify-content: center;
}

li {
    margin-right: 10px;
}
</style>