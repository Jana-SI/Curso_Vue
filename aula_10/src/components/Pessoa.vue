<template>
<p>Esta é a descrição da pessoa: {{nome}}</p>
<Info />   
</template>
<script>

import Info from './Info.vue';

    export default{
        name: 'Pessoa',
        components: {
    Info
  },
        data(){
            return{
                nome: 'Janaina'
            }
        }
    }
</script>