<script setup>
import { ref } from 'vue'

const count = ref(0)

const increment = () => {
  count.value++
}
</script>

<template>
  <button @click="increment" class="global-box increment-button">Increment</button>
  <h1>Count: {{ count }}</h1>
</template>

<style>
.increment-button {
  border: 0;
  background-color: hsl(160, 100%, 37%);
  color: white;
  font-size: 1.5rem;
}
</style>
