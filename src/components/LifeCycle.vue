<template>
    <h1>Meu nome é: {{ nome }}</h1>
</template>

<script>
export default {
    name: 'LifeCycle',
    data() {
        return {
            nome: 'Ainda não sei'
        }
    },
    created() {
        setTimeout(() => {
            this.nome = 'Pedro'
        }, 1000)       
    },
    mounted() {
        setTimeout(() => {
            this.nome = 'Pedro César'
        }, 2000)
    }

}
</script>