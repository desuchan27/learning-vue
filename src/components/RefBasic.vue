<script setup>
    import { onMounted, ref } from 'vue';

    const myInput = ref(null);

    onMounted(() => {
        // console.log(myInput.value);
        myInput.value.focus();
        myInput.value.value = 'something like that'
    })
</script>

<template>
    <input type="text" ref="myInput" />
    <p>{{ myInput }}</p>
</template>

<style scoped>
</style>