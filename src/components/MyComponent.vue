<!-- JS -->
<script setup>
import NestedComponent from './NestedComponent.vue'
console.log('Hello World')
</script>

<!-- HTML  -->
<template>
  <div>
    <h1>Hello World</h1>
    <NestedComponent />
  </div>
</template>

<!-- CSS  -->
<style scoped>
h1 {
  font-weight: 900;
  color: #999;
  text-align: center;
}
</style>
