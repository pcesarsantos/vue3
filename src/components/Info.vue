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
        <p>Para acessar meu Porfolio <a v-bind:href="meuLink" target="_blank">Basta clicar aqui</a></p>
        <myPicture />
    </div>
</template>
<script>
import myPicture from './Picture.vue'
export default {
    name: 'MyInfo',
    components: {
        myPicture
    },
    data() {
        return {
            estaTrabalhando: false,
            mostrarEmail: false,
            email: 'pcsantos@outlook.com.br',
            meuLink: 'http://www.github.com/pcesarsantos'
        }
    }
}
</script>