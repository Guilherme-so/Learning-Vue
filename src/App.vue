<script setup>
import Learning from "./components/Learning.vue";
import LifeCycle from "./components/LifeCycle.vue";
import Diretives from "./components/Diretives.vue";
import Dinamicos from "./components/Dinamicos.vue"
</script>

<template>
  <h1>Learning {{ skill }}</h1>
  <!-- <Learning /> -->
  <!-- <LifeCycle /> -->
  <!-- <Diretives /> -->

  <Dinamicos />
</template>

<script>
export default {
  data() {
    return {
      skill: "Vue",
    };
  },
  components: { Diretives },
};
</script>
