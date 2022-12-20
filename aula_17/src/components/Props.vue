<template>
    <p>{{ txt }}</p>
    <p v-if="ShoworHide">Sou Boolean!</p>
</template>

<script>
export default{
    name: 'Props',
    props: {
        txt: String,
        ShoworHide: Boolean
    }
}
</script>