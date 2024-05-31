<script setup>
import MyComponent from './components/MyComponent.vue'
import CombinedStyle from './components/CombinedStyle.vue'
import ModuleStyle from './components/ModuleStyle.vue'
import MyEvent from './components/MyEvent.vue'
import MyReactiveComponent from './components/MyReactiveComponent.vue'
import MyRefComponent from './components/MyRefComponent.vue'
import IterationComponent from './components/IterationComponent.vue'
import BindingComponent from './components/BindingComponent.vue'
// import GlobalStyle from './components/GlobalStyle.vue'
// import LocalStyle from './components/LocalStyle.vue'
</script>
<template>
  <!-- <GlobalStyle />
  <LocalStyle /> -->
  <MyComponent />
  <CombinedStyle />
  <ModuleStyle />
  <MyEvent />
  <MyReactiveComponent />
  <MyRefComponent />
  <IterationComponent />
  <BindingComponent />
</template>
<style scoped>
/* h1 {
  font-weight: 900;
  color: #999;
  text-align: center;
} */
</style>
