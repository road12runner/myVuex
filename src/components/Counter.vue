<template>
  <div>
    <button class="btn btn-primary" @click="increment">Increment</button>
    <button class="btn btn-primary" @click="decrement">Decrement</button>
  </div>
</template>

<script>
  export default {
    methods: {
      increment() {
        this.$store.state.counter++;
        //this.$emit('updated', 1);
      },
      decrement() {
        //this.$emit('updated', -1);
        this.$store.state.counter--;
      }
    }
  }
</script>

<style>
</style>