<script setup>
import { useCounter } from '@/composables/useCounter';

const counter = useCounter()
</script>

<template>
    <h1>{{ count }}</h1>
    <button @click="counter.increment">+</button>
    <button @click="counter.decrement">-</button>
</template>