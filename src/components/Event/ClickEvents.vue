<template>
    <h1>{{ age }}</h1>

    <button type="button" @click="decrementHandler">Decrement</button>
    <button type="button" @click.ctrl="age++">Increment</button>
</template>

<script>
export default {
    data(){
        return {
            age: 20
        }
    },
    methods: {
        decrementHandler(){
            this.age--
        }
    }
}

</script>