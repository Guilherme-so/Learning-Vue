<script setup>
import Learning from "./components/Learning.vue";
import LifeCycle from "./components/LifeCycle.vue";
import Diretives from "./components/Diretives.vue";
import Dinamicos from "./components/Dinamicos.vue";
import Methods from "./components/Methods.vue";
import Header from "./components/Header.vue";
import Forms from "./components/Forms.vue";
import Multiplos_eventos from "./components/Multiplos_eventos.vue";
</script>

<template>
  <Header logo="Learning Vue.js" :logado=true :perfil="perfil" />
  <!-- <Learning /> -->
  <!-- <LifeCycle /> -->
  <!-- <Dinamicos /> -->
  <!-- <Methods /> -->
  <!-- <Diretives /> -->
  <!-- <Forms /> -->
  <Multiplos_eventos />
</template>

<script>
export default {
  data() {
    return {
      perfil: "Guilherme",
    };
  },
  components: { Header, Forms, Multiplos_eventos },
};
</script>

<style>
body {
  background-color: #ddd;
  color: #fff;
}

a {
  text-decoration: none;
  color: #ddd;
}

</style>
