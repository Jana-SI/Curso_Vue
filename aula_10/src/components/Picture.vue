<template>
    <img class="rounded float-start" :src="avatar" :alt="descricao">
</template>

<script>
export default {
    name: 'Picture',
    data() {
        return {
            avatar: "/img/avatar.png",
            descricao: "img de avatar"
        }
    }
}
</script>

<style>
img{ margin: 10px;}
</style>