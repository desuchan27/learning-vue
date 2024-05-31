<script setup>
defineProps({
  friends: Array,
  userInfo: Object
})
</script>

<template>
  <!-- <h1>{{ friends }}</h1> -->
  <h1>{{ userInfo }}</h1>

  <ul v-for="(friend, index) in friends" :key="index">
    <li>{{ friend }}</li>
  </ul>
</template>
