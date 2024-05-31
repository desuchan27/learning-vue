<script setup>
import { ref } from 'vue'

const props = defineProps(['name'])
</script>

<template>
  <h1>Hello, {{ props.name }}</h1>
</template>
