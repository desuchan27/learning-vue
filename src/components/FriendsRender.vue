<script setup>
import { ref } from 'vue'
const friends = ref(['Desu', 'JS', 'Chan'])
</script>

<template>
    <p v-for="(friend, i) in friends" :key="i">{{ friend }} </p>
</template>