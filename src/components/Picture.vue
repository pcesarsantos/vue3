<template>
    <img :src="avatar" :alt="descricao">
</template>
<script>
export default {
    name: 'myPicture',
    data() {
        return {
            avatar: "/img/avatar.jpg",
            descricao: "Pedro César"
        }
    }
}
</script>