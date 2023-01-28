<template>
  <div class="container">
    <h2>Multiplos Eventos</h2>
    <p>{{ eventos }}</p>
    <button
      @click="
        primeiro($event), segundo($event), terceiro($event), quarto($event)
      "
    >
      Enviar
    </button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      eventos: "",
    };
  },
  methods: {
    primeiro(e) {
      this.eventos = "Primeiro Evento...";
    },
    segundo(e) {
      setTimeout(() => {
        this.eventos = "Segundo Evento...";
      }, 1000);
    },
    terceiro(e) {
      setTimeout(() => {
        this.eventos = "Terceiro Evento...";
      }, 1500);
    },
    quarto(e) {
      setTimeout(() => {
        this.eventos = "";
      }, 2000);
    },
  },
};
</script>

<style scoped>
.container {
  display: flex;
  margin: auto;
  align-items: center;
  justify-content: center;
}
</style>
