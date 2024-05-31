<script setup>
import { ref } from 'vue'
import MyComponent from './components/MyComponent.vue'
import CombinedStyle from './components/CombinedStyle.vue'
import ModuleStyle from './components/ModuleStyle.vue'
import MyEvent from './components/MyEvent.vue'
import MyReactiveComponent from './components/MyReactiveComponent.vue'
import MyRefComponent from './components/MyRefComponent.vue'
import IterationComponent from './components/IterationComponent.vue'
import BindingComponent from './components/BindingComponent.vue'
import StaticPropsComponent from './components/StaticPropsComponent.vue'
import DynamicPropsComponent from './components/DynamicPropsComponent.vue'
import ChangingPropsValue from './components/ChangingPropsValue.vue'
import PropValidation from './components/PropValidation.vue'
// import GlobalStyle from './components/GlobalStyle.vue'
// import LocalStyle from './components/LocalStyle.vue'

const firstName = ref('Desu')
const lastName = ref('JS')
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
  <StaticPropsComponent name="John Doe" />
  <DynamicPropsComponent :firstName="firstName" :lastName="lastName" />
  <ChangingPropsValue />
  <PropValidation fullName="Desu Chan" :age="21" />
</template>
<style scoped>
/* h1 {
  font-weight: 900;
  color: #999;
  text-align: center;
} */
</style>
