<template>
<form action="" @submit="enviarFormulario">
    <div>
        <input type="Text" v-model="name">
    </div>
    <div>
        <input type="text" v-model="email">
    </div>
    <div>
        <InputSubmit />
    </div>
</form>
</template>

<script>
// import InputText from './Form/InputText.vue'
import InputSubmit from './Form/InputSubmit.vue'

export default {
    name: "MyForm",
    components: {
        // InputText,
        InputSubmit
    },
    data() {
        return {
            name: "",
            email: ""
        }
    },
    methods: {
        enviarFormulario(e) {
            e.preventDefault()

            console.log(`O nome é ${this.name} e o email é ${this.email}`)
            console.log('Formulario enviado')
        }
    }
}
</script>