<script setup>
import { ref } from 'vue'

const username = ref('')
const email = ref('')
const password = ref('')
</script>

<template>
  <form @submit.prevent="$emit('userInfo', username, email, password)">
    <label for="username">Username</label>
    <input type="text" id="username" v-model="username" />
    <label for="email">Email</label>
    <input type="email" id="email" v-model="email" />
    <label for="password">Password</label>
    <input type="password" id="password" v-model="password" />
    <button type="submit">Submit</button>
  </form>
</template>
