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
        this.lifeClycle('Created')
    },
    mounted() {
        setTimeout(() => {
            this.nome = 'Pedro César'
        }, 2000)
        this.lifeClycle('Mounted')
    },
    methods: {
        lifeClycle(mensagem) {
            console.log(`etapa: ${mensagem}`)
        }
    }

}
</script>