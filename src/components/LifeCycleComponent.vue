<script setup>
import {
  ref,
  onBeforeMount,
  onMounted,
  onBeforeUpdate,
  onUpdated,
  onBeforeUnmount,
  onUnmounted
} from 'vue'

const message = ref('Hello, Vue 3!')

onMounted(() => {
  console.log('Component has been mounted')
})

onBeforeMount(() => {
  console.log('Component is about to be mounted')
})

onBeforeUpdate(() => {
  console.log('Component is about to update')
})

onUpdated(() => {
  console.log('Component has been updated')
})

const updateMessage = () => {
  message.value = 'Hello, Vue 3! (updated)'
}

onBeforeUnmount(() => {
  console.log('Component is about to be unmounted')
})
</script>

<template>
  <div class="cols">
    <p class="text-center space-y">{{ message }}</p>
    <button class="global-button global-box" @click="updateMessage">update message</button>
  </div>
</template>
