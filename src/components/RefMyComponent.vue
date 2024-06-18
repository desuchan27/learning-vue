<script setup>

import { defineExpose, ref } from 'vue'

// When using the script setup
// - it's private by default
// - A parent referencing to a child won't be able to access anything.

// First we have to expose all the properties and methods.
// then we'd be able to use them in parent component.
// - use (defineExpose) to expose our data for the parent to use.

const count = ref(10)

const increment = () => {
    count.value++
}

const decrement = () => {
    count.value--
}

defineExpose({ count, increment, decrement })
</script>

<template>
    <div>
        <h1>Ref My Component</h1>
        <p>Count: {{ count }}</p>
        <button @click="increment">Increment</button>
        <button @click="decrement">Decrement</button>
    </div>
</template>