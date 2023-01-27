<template>
  <h1>Dados dinamicos</h1>
  <p>
    Segue o link para o site
    <a v-bind:href="link_externo" target="_blank"> Clickando aqui</a>
  </p>
  <img :src="avatar" :alt="avatar_alt" />
</template>

<script>
export default {
  data() {
    return {
      link_externo: "https://google.com",
      avatar: "https://github.com/Guilherme013S.png",
      avatar_alt: "github avatar",
    };
  },
};
</script>
