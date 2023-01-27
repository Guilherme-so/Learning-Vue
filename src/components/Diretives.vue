<template>
  <h4 v-if="estou_com_preguiça">Watch Youtube, Listen to music and play chess</h4>
  <h4 v-else>Estudar programaçao</h4>
  <br>

  <div>
    <h1>v-show se for verdade mostra se nao, nao mostra nada</h1>
      <h3 v-show="show_password">{{ password }}</h3>
  </div>
</template>

<script>
export default {
  data() {
    return {
        'estou_com_preguiça' : false,
        'password': "gui12345",
        'show_password' : true
    };
  },
};
</script>
