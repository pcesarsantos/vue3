<template>
    <div>
        <p v-if="estaTrabalhando">Estou trabalhando no momento.</p>
        <p v-else>Estou em busca de novas oportunidades</p>
        <p>utilizo as seguintes tecnologias:</p>
        <ul>
            <li>Javascript</li>
            <li>PHP</li>
            <li>C#</li>
        </ul>
        <p v-show="mostrarEmail">Mande uma mensagem para {{email}}</p>
    </div>
</template>
<script>
export default {
    name: 'MyInfo',
    data() {
        return {
            estaTrabalhando: false,
            mostrarEmail: false,
            email: 'pcsantos@outlook.com.br'
        }
    }
}
</script>