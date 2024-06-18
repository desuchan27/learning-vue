<script setup>
import GlobalStyle from './components/GlobalStyle.vue'
import { ref } from 'vue'
import CounterComponentAlso from './components/CounterComponentAlso.vue'
import CounterComponent from './components/CounterComponent.vue'
// import FriendsToggle from './components/FriendsToggle.vue'
// import RefComponent from './components/RefComponent.vue'
// import BasicRef from './components/RefBasic.vue';
// import MyComponent from './components/MyComponent.vue'
// import CombinedStyle from './components/CombinedStyle.vue'
// import ModuleStyle from './components/ModuleStyle.vue'
// import MyEvent from './components/MyEvent.vue'
// import MyReactiveComponent from './components/MyReactiveComponent.vue'
// import MyRefComponent from './components/MyRefComponent.vue'
// import IterationComponent from './components/IterationComponent.vue'
// import BindingComponent from './components/BindingComponent.vue'
// import StaticPropsComponent from './components/StaticPropsComponent.vue'
// import DynamicPropsComponent from './components/DynamicPropsComponent.vue'
// import ChangingPropsValue from './components/ChangingPropsValue.vue'
// import PropValidation from './components/PropValidation.vue'
// import ComplexPropsComponent from './components/ComplexPropsComponent.vue'
// import CustomValidator from './components/CustomValidator.vue'
// import ComponentEvent from './components/ComponentEvent.vue'
// import FromComponent from './components/FromComponent.vue'
// import SlotComponent from './components/SlotComponent.vue'
// import FallbackComponent from './components/FallbackComponent.vue'
// import NamedSlot from './components/NamedSlot.vue'
// import SchoolComponent from './components/SchoolComponent.vue'
// import SchoolComponent from './components/SchoolComponent.vue'
// import LocalStyle from './components/LocalStyle.vue'
// import LifeCycleComponent from './components/LifeCycleComponent.vue'
// import RefFunction from './components/RefFunction.vue';

import { provide } from 'vue'

// const firstName = ref('Desu')
// const lastName = ref('JS')
// const count = ref(0)

// const formHandler = (username, email, password) => {
//   console.log(username, email, password)
// }

// const studentName = 'Desu Chan'
// const studentAge = 21
// const studentLocation = 'Philippines'

const value = ref(0)

provide('studentName', 'Desu Chan')
provide('studentAge', 21)
provide('studentLocation', 'Philippines')

// const showHide = ref(true)
</script>
<template>
  <GlobalStyle>
    <!-- <GlobalStyle />
  <LocalStyle /> -->
    <!-- <MyComponent />
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
  <ComplexPropsComponent
    :friends="['Gon', 'Killua', 'Kurapika', 'Leorio']"
    :userInfo="{ name: 'Desu', age: 21, location: ['Philippines'] }"
  />
  <CustomValidator name="Da Wei" age:20 password="real123456789" />
  <h1>Count: {{ count }}</h1>
  <ComponentEvent @incrementCounter="count++" />
  <FromComponent @userInfo="formHandler" />
  <SlotComponent>
    <h2>Content 1</h2>
    <h2>Content 2</h2>
  </SlotComponent>
  <FallbackComponent> </FallbackComponent>
  <NamedSlot>
    <template #one>
      <h2>Content Slot 1</h2>
    </template>
<template #two>
      <h2>Content Slot 2</h2>
    </template>
</NamedSlot> -->
    <!-- <SchoolComponent /> -->
    <!-- <LifeCycleComponent v-if="showHide" />
    <button @click="showHide = !showHide">Toggle</button> -->
    <!-- <BasicRef /> -->
    <!-- <RefFunction /> -->
    <!-- <RefFunction /> -->
    <!-- <RefComponent /> -->
    <!-- <FriendsToggle /> -->
    <CounterComponent />
    <CounterComponentAlso />
  </GlobalStyle>
</template>
<style scoped>
/* h1 {``````````````````````````
  font-weight: 900;
  color: #999;
  text-align: center;
} */
</style>
