<script setup>
// import FriendsRender from './FriendsRender.vue'
import { defineAsyncComponent, ref } from 'vue'
const FriendsRender = defineAsyncComponent(() => import('./FriendsRender.vue'))

const showFriends = ref(false)

const toggleFriends = () => {
    showFriends.value = !showFriends.value
}

</script>

<template>
    <div v-if="showFriends">
        <FriendsRender />
    </div>
    <button @click="toggleFriends">Toggle Friends</button>
</template>