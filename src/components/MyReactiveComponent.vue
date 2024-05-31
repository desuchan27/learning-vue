<script setup>
import { reactive } from 'vue'
let initialState = reactive({ count: 0 })
</script>

<template>
  <div class="rows">
    <button @click="initialState.count++" class="increment-button global-box">Increment</button>
    <button @click="initialState.count++" class="increment-button global-box">Increment</button>
  </div>
  <h1>Count: {{ initialState.count }}</h1>
</template>
