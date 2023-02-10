<template>
  <div class="if_else">
    <h4 v-if="music === 1">
      I' gonna listen to Perl jam 
    </h4>
    <h4 v-else-if="music === 2">
      I' gonna listen to Gorrilaz       
    </h4>
    <h4 v-else>Im not gonna listen to music now</h4>
  </div>
  <br />

  <div class="v_show">
    <h1>v-show display just if its true</h1>
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
      music: 3,
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
