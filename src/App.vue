<template>
  <div>
    <myHeader />
    <PrimeiroComponente />
    <p class="paragrafo-pai">
      o dado de app é: {{ testando }}
    </p>
    <LifeCycle />
    <Pessoa />
  </div>
</template>

<script>
import myHeader from './components/myHeader.vue'
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa.vue'

export default {
  name: 'App',
  components: {
    myHeader,
    PrimeiroComponente,
    LifeCycle,
    Pessoa
  },
  data() {
    return {
      testando: "Teste"
    }
  }
}
</script>

<style>
  body {
    background-color: #333;
    color: #fff;
  }

  a {
    color: red;
  }

  .teste {
    background-color: #000;
  }
</style>