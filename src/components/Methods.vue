<template>
  <h1>Metodos</h1>

  <div>
    <p v-show="modal">Modal Opened</p>

    <button @click="toogleModal">
      {{ modal === true ? "Close Modal" : "Open Modal" }}
    </button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      modal: true,
    };
  },
  methods: {
    toogleModal() {
      this.modal = !this.modal;
      console.log('clicked')
    },
  },
};
</script>
