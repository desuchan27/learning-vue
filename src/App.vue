<script setup>
import MyComponent from './components/MyComponent.vue'
import CombinedStyle from './components/CombinedStyle.vue'
import ModuleStyle from './components/ModuleStyle.vue'
// import GlobalStyle from './components/GlobalStyle.vue'
// import LocalStyle from './components/LocalStyle.vue'
</script>
<template>
  <!-- <GlobalStyle />
  <LocalStyle /> -->
  <MyComponent />
  <CombinedStyle />
  <ModuleStyle />
</template>
<style scoped>
/* h1 {
  font-weight: 900;
  color: #999;
  text-align: center;
} */
</style>
