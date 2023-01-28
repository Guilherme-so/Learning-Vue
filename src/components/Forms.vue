<template>
  <div class="container">
    <h2>Meu Formulario</h2>

    <form @submit="handleSubmit($event)">
      <div>
        <input type="text" placeholder="Nome" v-model="nome" />
      </div>
      <div>
        <input type="text" placeholder="Email" v-model="email" />
      </div>

      <button type="submit">Enviar</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      nome: "",
      email: "",
    };
  },
  methods: {
    handleSubmit(e) {
      e.preventDefault();

      const nome = this.nome;
      const email = this.email;

      console.log(nome);
      console.log(email);
      this.nome = "";
      this.email = "";
    },
  },
};
</script>

<style>
.container {
    display: flex;
    flex-direction: column;
    margin: 0 auto;
    justify-content: center;
    align-items: center;
}
</style>