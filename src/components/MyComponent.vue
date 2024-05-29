<!-- JS -->
<script setup>
import NestedComponent from './NestedComponent.vue'

const name = 'Desu JS'
</script>

<!-- HTML  -->
<template>
  <div>
    <h1>{{ name }}</h1>
    <NestedComponent />
  </div>
</template>

<!-- CSS  -->
<style scoped>
h1 {
  font-weight: 900;
  color: #999;
}
</style>
