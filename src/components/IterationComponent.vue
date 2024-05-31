<script setup>
import { ref } from 'vue'

const people = ref([
  { name: 'John', age: 30 },
  { name: 'Jane', age: 25 },
  { name: 'Susan', age: 35 }
])
</script>

<template>
  <div class="rows global-box">
    <p v-for="(person, index) in people" :key="index">
      {{ person.name }} is {{ person.age }} years old
    </p>
  </div>
</template>
