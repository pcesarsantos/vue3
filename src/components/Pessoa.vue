<template>
    <div>
        <h2>Esta é a descrição da pessoa: {{ nome }}</h2>
        <Info />
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
            nome: 'Pedro'
        }
    }
}
</script>
