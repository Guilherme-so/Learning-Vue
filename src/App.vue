<script setup>
import Learning from "./components/Learning.vue";
import LifeCycle from "./components/LifeCycle.vue";
import Diretives from "./components/Diretives.vue";
import Dinamicos from "./components/Dinamicos.vue";
import Methods from "./components/Methods.vue";
import Header from "./components/Header.vue";
import Forms from "./components/Forms.vue";
import Multiplos_eventos from "./components/Multiplos_eventos.vue";
import ClickEvents from "./components/Event/ClickEvents.vue";
import ChangeEvent from "./components/Event/ChangeEvent.vue";
</script>

<template>
  <Header logo="Learning Vue.js" :logado=true :perfil="perfil" />
  <div id="container">
    <!-- <Learning /> -->
    <!-- <LifeCycle /> -->
    <!-- <Dinamicos /> -->
    <!-- <Methods /> -->
    <!-- <Diretives /> -->
    <!-- <Forms /> -->
    <!-- <Multiplos_eventos /> -->
    <!-- <ClickEvents /> -->
    <ChangeEvent />
  </div>
</template>

<script>
export default {
  data() {
    return {
      perfil: "Guilherme",
    };
  },
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

#container {
  display: flex;
  flex-direction: column;
  margin: 0 auto;
  align-items: center;
  justify-content: center;
}

</style>
