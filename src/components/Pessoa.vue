<template>
    <div>
        <h2>Esta é a descrição da pessoa: {{ nome }}</h2>
        <Info :email="email" :estaTrabalhando="estaTrabalhando" />
    </div>
    <div>
        <myForm />
    </div>
</template>
<script>
import Info from './Info.vue'
import myForm from './myForm.vue'

export default {   
    name: 'MyPessoa',
    components: {
        Info,
        myForm
    },
    data() {
        return {
            nome: 'Pedro',
            email: 'pcsantos@outlook.com.br',
            estaTrabalhando: false
        }
    }
}
</script>
