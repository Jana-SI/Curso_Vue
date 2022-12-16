<template>
    <div>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Link 01</a></li>
        <li><a href="#">Link 02</a></li>
    </ul>
</div>
</template>

<script>
export default{
    name: 'Header'
}
</script>

<style scoped>
ul{
    list-style: none;
    display: flex;
    justify-content: center;
    background-color: #37495f;
    padding: 10px;
}

li{
    margin-right: 10px;
}

a{
    color: white !important;
    text-decoration: none;
    transition: .5s;
}

a:hover{
    color: green  !important;
}
</style>