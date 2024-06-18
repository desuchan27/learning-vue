<script setup>
import RefMyComponent from './RefMyComponent.vue'
import { onMounted, ref } from 'vue'

const myRef = ref(null)

onMounted(() => {
    console.log(myRef.value)
})
</script>

<template>
    <RefMyComponent ref="myRef" />
</template>