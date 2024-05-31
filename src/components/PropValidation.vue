<script setup>
const props = defineProps({
  fullName: {
    type: String,
    required: true
  },
  age: {
    type: Number,
    required: true
  }
})
</script>

<template>
  <div class="rows">
    <h1>{{ props.fullName }}</h1>
    <h1>{{ props.age }}</h1>
  </div>
</template>
