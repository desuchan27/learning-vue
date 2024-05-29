<script setup>
const age = 21
const occupation = 'Web Developer'
const bio = 'I aim to be productive each day (except Sundays 😜).'
const githubLink = 'https://github.com/desuchan27'
</script>

<template>
  <p>{{ age }}</p>
  <p>{{ occupation }}</p>
  <p>{{ bio }}</p>
  <a :href="githubLink" target="_blank">GitHub</a>
</template>

<style scoped></style>
