<script setup>
import { ref } from 'vue'

import DComponentOne from './DComponentOne.vue'
import DComponentTwo from './DComponentTwo.vue'
import DComponentThree from './DComponentThree.vue'

const activeComponent = ref('DComponentOne')

const components = {
    DComponentOne,
    DComponentTwo,
    DComponentThree
}

// const changeComponent = (component) => {
//     activeComponent.value = component
// }

</script>

<template>
    <div>
        <button @click="activeComponent = 'DComponentOne'">HTML</button>
        <button @click="activeComponent = 'DComponentTwo'">CSS</button>
        <button @click="activeComponent = 'DComponentThree'">JS</button>

        <component :is="components[activeComponent]" />

    </div>
</template>