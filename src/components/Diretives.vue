<template>
  <div class="if_else">
    <h4 v-if="estou_com_preguiça">
      Watch Youtube, Listen to music and play chess
    </h4>
    <h4 v-else>Estudar programaçao</h4>
  </div>
  <br />

  <div class="v_show">
    <h1>v-show se for verdade mostra se nao, nao mostra nada</h1>
    <h3 v-show="show_password">{{ password }}</h3>
  </div>

  <div class="loop">
    <h2>Tecnologies frontend Loop</h2>
    <ul>
      <li v-for="(tecnology, index) in tecnologies" :key="index">
        {{ tecnology }}
      </li>
    </ul>
  </div>

  <div class="loop">
    <h2>Tecnologies Backend Loop</h2>
    <ul>
      <li v-for="tecnology in tecnologies_backend" :key="tecnology.id">
        {{ tecnology.name }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      estou_com_preguiça: false,
      password: "gui12345",
      show_password: true,
      tecnologies: ["React", "Vue", "Angular"],
      tecnologies_backend: [
        {
          id: 1,
          name: "Express",
        },
        { id: 2, name: "Django" },
        {
          id: 3,
          name: "Lavarel",
        },
      ],
    };
  },
};
</script>

<style>
.if_else {
  background-color: yellow;
}

.v_show {
  background-color: greenyellow;
}

.loop {
  background-color: orangered;
}
</style>
