<template>
    <div>
        <button @click="primeiro(), segundo(), terceiro()">Ativar Multiplos Eventos</button>
        <p> {{ multiplosEventos }}</p>
    </div>
</template>

<script>
export default {
    name: "MultiplosEventos",
    data() {
        return {
            multiplosEventos: ""
        }
    },
    methods: {
        primeiro() {
            this.multiplosEventos = "Primeiro evento ativado"
        },
        async segundo() {
            setTimeout(() => { this.multiplosEventos = "Segundo Evento ativado"}, 500)
        },
        async terceiro() {
            setTimeout(() => { this.multiplosEventos = ""}, 1500)
        }
    }
}
</script>
<style scoped>
div {
    margin: 100px;
}
</style>