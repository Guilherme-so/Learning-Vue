<script setup>
import Learning from "./components/Learning.vue";
import LifeCycle from "./components/LifeCycle.vue";
import Diretives from "./components/Diretives.vue";
import Dinamicos from "./components/Dinamicos.vue"
import Methods from "./components/Methods.vue";
import Header from "./components/Header.vue";

</script>

<template>
  <Header/>

<h1>Learning {{ skill }}</h1>
  <!-- <Learning /> -->
  <!-- <LifeCycle /> -->
  <!-- <Dinamicos /> -->
  <!-- <Methods /> -->
  <Diretives />
</template>

<script>
export default {
    data() {
        return {
            skill: "Vue",
        };
    },
    components: { Header }
};
</script>


<style>

body{
  background-color: #ddd;
  color: #fff;
}

</style>