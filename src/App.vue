<script setup>
  import {ref} from 'vue'
  let count = ref(0)
  const incrementCounter = () => count.value++
  const decrementCounter = () => count.value--
</script>

<template>
  <main>
    <h1>Vue Counter</h1>
    <h3 >{{count}}</h3>
    <div><button class="actions" @click="decrementCounter"> - </button><button class="actions" @click="incrementCounter"> + </button></div>
  </main>
</template>

<style scoped>
  span {
    border: solid, 5px;
    border-radius: 2px;
    padding: 20px;
  }
</style>