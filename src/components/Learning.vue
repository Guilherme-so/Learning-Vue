<template>
  <p>I'm {{ multi === true ? "Gui" : "Guilherme"}} and I'm learning {{ skills }}</p>
</template>

<script>
export default {
  data() {
    return {
      nome: "Guilherme",
      skills: "React and Vue",
      multi: false
    };
  },
};
</script>
