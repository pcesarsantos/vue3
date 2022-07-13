<template>
    <div>
        <img :src="avatar" :alt="descricao" />
        <MudarImagem @mudarImagem="trocarImagem" />
    </div>
</template>
<script>
import MudarImagem from './MudarImagem.vue'
export default {
    name: 'myPicture',
    components: {
        MudarImagem
    },
    data() {
        return {
            avatar: "/img/avatar.jpg",
            descricao: "Pedro César"
        }
    },
    methods: {
        trocarImagem() {
            this.avatar = '/img/avatar2.png'
        }
    }
}
</script>