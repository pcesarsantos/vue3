<template>
    <div>
        <img :src="avatar" :alt="descricao" />
        <Reutilizacao />
    </div>
</template>
<script>
import Reutilizacao from './Reutilizacao.vue'
export default {
    name: 'myPicture',
    components: {
        Reutilizacao
    },
    data() {
        return {
            avatar: "/img/avatar.jpg",
            descricao: "Pedro César"
        }
    }
}
</script>