<template>
    <div>
        <h2>Esta é a descrição da pessoa: {{ nome }}</h2>
        <Info />
    </div>
</template>
<script>
import Info from './Info.vue'

export default {   
    name: 'MyPessoa',
    components: {
        Info
    },
    data() {
        return {
            nome: 'Pedro'
        }
    }
}
</script>
