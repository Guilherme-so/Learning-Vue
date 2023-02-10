<template>
  <h1>Biding classes and styles</h1>

  <div class="check">
    <input type="checkbox" id="purple" v-model="isPurple" />
    <label for="purple">Purple</label>
  </div>

  <select v-model="selectedColor">
    <option value="">None</option>
    <option value="white">White</option>
    <option value="orange">Orange</option>
    <option value="pink">Pink</option>
    <option value="blue">Blue</option>
  </select>

  <div 
  :style="{ width: size + 'px', height: size + 'px' }"
  class="hi" :class="[isPurple ? 'purple' : '', selectedColor]">H1</div>

  <input
    type="number"
    v-model="size"
  />
</template>

<script>
export default {
  data() {
    return {
      isPurple: true,
      selectedColor: "",
      size: 200,
    };
  },
};
</script>

<style scoped>
.hi {
  width: 200px;
  height: 200px;
  background-color: green;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
  margin: 20px 0;
}
.check {
  display: flex;
  margin-bottom: 20px;
}

.purple {
  background-color: purple;
}

.white {
  background-color: #fff;
}

.orange {
  background-color: orangered;
}

.pink {
  background-color: pink;
}

.blue {
  background-color: blue;
}
</style>
>
