<template>
  <h1>Hello Vue 3!</h1>
  <button @click="inc">Clicked {{ count }} times.</button>
</template>

<script>
import { ref } from 'vue'
export default {
  setup() {
    const count = ref(0)
    const inc = () => {
      count.value++
    }
    return {
      count,
      inc
    }
  },
  mounted() {
    console.log(1111);
    console.log(this);
  },
}
</script>

<style scoped>
h1 {
  font-family: Arial, Helvetica, sans-serif;
}
</style>