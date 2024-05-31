<script setup>
import { ref } from 'vue'
const formData = ref({
  name: '',
  age: ''
})

// const submitForm = (e) => {
//   e.preventDefault()
//   console.log('Name:', formData.value.name)
//   console.log('Age:', formData.value.age)
// }
</script>

<template>
  <form>
    <div class="rows">
      <label>Name</label>
      <input
        class="global-box"
        type="text"
        placeholder="Please enter your name"
        v-model="formData.name"
      />
      <label>Age</label>
      <input
        class="global-box"
        type="text"
        placeholder="Please enter your age"
        v-model="formData.age"
      />
    </div>
    <!-- <button class="global-box increment-button" @:click="submitForm">Submit</button> -->
  </form>
  <div class="rows">
    <p>Name: {{ formData.name }}</p>
    <p>Age: {{ formData.age }}</p>
  </div>
</template>
