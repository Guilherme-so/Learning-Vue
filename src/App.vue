<script setup>
import Learning from "./components/Learning.vue";
import LifeCycle from "./components/LifeCycle.vue";
</script>

<template>
  <h1>Learning {{ skill }}</h1>
  <Learning />

  <LifeCycle/>
</template>

<script>
export default {
  data() {
    return {
      skill: "Vue",
    };
  },
};
</script>
