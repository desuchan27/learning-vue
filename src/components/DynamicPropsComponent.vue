<script setup>
const props = defineProps(['firstName', 'lastName'])
</script>

<template>
  <h1>Hello, {{ props.firstName }} {{ props.lastName }}</h1>
</template>
