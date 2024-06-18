<script setup>
const myRefFunc = (element) => {
    console.log(element.textContent)
    element.textContent = 'This is the updated value'
    element.style
}
</script>

<template>
    <h1 :ref="myRefFunc">This is the initial value</h1>
</template>