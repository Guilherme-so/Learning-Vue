<template>
  <h1>
    {{ printName() }}
    <hr />
    <p>Idade: {{ age }}</p>
  </h1>

  <label for="firstName">First Name:</label>
  <input type="text" id="firstName" v-model.lazy.trim="firstName" />

  <label for="middleName">Middle Name:</label>
  <input type="text" id="middleName" @keyup.enter="middleNameHandleChange" />

  <label for="lastName">Last Name:</label>
  <input
    type="text"
    id="lastName"
    :value="lastName"
    @input.prevent="lastNameHandleChange('event trigged', $event)"
  />

  <label for="age">Age:</label>
  <input type="number" v-model.number="age" />
</template>

<script>
export default {
  data() {
    return {
      firstName: "Guilherme",
      middleName: "",
      lastName: "Oliveira",
      age: 20,
    };
  },
  methods: {
    printName() {
      return `${this.firstName} ${this.middleName} ${this.lastName}`;
    },
    middleNameHandleChange(event) {
      this.middleName = event.target.value;
    },
    lastNameHandleChange(msg, event) {
      // commentei o preventDefault pq to usando event modifier direto no input
      //   event.preventDefault();
      console.log(msg);
      this.lastName = event.target.value;
    },
  },
  watch: {
    age(newAge, oldAge){
        setTimeout(() => {
            this.age = 20
        }, 3000)
    }
  }
};
</script>
