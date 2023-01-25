<template>
  <p>I'm {{ nome }} and I'm learning {{ skills }}</p>
</template>

<script>
export default {
  data() {
    return {
      nome: "Guilherme",
      skills: "React and Vue",
    };
  },
};
</script>