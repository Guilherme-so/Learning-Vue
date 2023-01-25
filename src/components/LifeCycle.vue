<template>
  <h1>Let's undestand lifecycle of vue</h1>
  <p>Here's my data: {{ data }}</p>
</template>

<script>
export default {
  data() {
    return {
      data: "First data",
    };
  },
  created() {
    setTimeout(() => {
      this.data = "Second Data";
    }, 1000);
  },

  mounted() {
    setTimeout(() => {
      this.data = "Third Data";
    }, 2000);
  },
};
</script>
