<script setup>
import { ref } from 'vue'
let username = ref('No username set yet')
</script>

<template>
  <h1>{{ username }}</h1>
  <button @click="username = 'desuchan27'" class="increment-button global-box">Set Username</button>
</template>
