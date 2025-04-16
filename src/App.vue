<template>
    <barramenu></barramenu> <!--Barra de menu mesclado ao header do site-->
    <paginaInicial></paginaInicial> <!--Página inicial, todo o conteúdo-->
</template>

<script>

import paginaInicial from './pages/homePage/paginaInicial.vue';
import barramenu from './components/menu/barramenu.vue';

export default {
  name: 'App',
  components: {
    barramenu,
    paginaInicial,
  }
}
</script>

<style>
#app{
  font-family: "Poppins", Helvetica, Arial, sans-serif;
  color: #ffffff;
  margin: 0;
  padding: 0;
}
</style>
