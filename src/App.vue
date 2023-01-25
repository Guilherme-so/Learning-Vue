<script setup>
import Learning from "./components/Learning.vue";
</script>

<template>
  <h1>Learning {{ skill }}</h1>
  <Learning />
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
