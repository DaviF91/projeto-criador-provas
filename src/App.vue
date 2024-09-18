<template>
  <PageBody msg="Welcome to Your Vue.js App"/>
</template>

<script>
import PageBody from './components/PageBody.vue'

export default {
  name: 'App',
  components: {
    PageBody
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0; /* Remova o margin-top se quiser que o conteúdo ocupe toda a altura da tela */
  width: 100vw; /* 100% da largura da viewport */
  height: 100vh; /* 100% da altura da viewport */
  display: flex;
  justify-content: center; /* Alinha horizontalmente o conteúdo no centro */
  align-items: center; /* Alinha verticalmente o conteúdo no centro */
  background: linear-gradient(to bottom right, #e0e0e0, #ffffff);
}
</style>
