<script setup>
// import GlobalStyle from './GlobalStyle.vue'
import { inject } from 'vue'

const studentName = inject('studentName')
const studentAge = inject('studentAge')
const studentLocation = inject('studentLocation')
</script>

<template>
  <div class="columns global-box">
    <h1>Student Component</h1>
    <h1>{{ studentName }}</h1>
    <p>Age: {{ studentAge }}</p>
    <p>Location: {{ studentLocation }}</p>
  </div>
</template>
