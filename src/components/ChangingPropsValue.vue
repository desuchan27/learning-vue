<script setup>
const props = defineProps(['favoriteNumber'])

// props.favoriteNumber = 10
</script>

<template>
  <h1>{{ props.favoriteNumber }}</h1>
</template>
