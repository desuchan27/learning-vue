<script setup>
import { ref } from 'vue'

const count = ref(0)
const inputValue = ref('')

const increment = () => {
  const value = Number(inputValue.value)
  if (isNaN(value)) {
    alert('Please enter a valid number')
    return
  }

  count.value += value
}

const decrement = () => {
  const value = Number(inputValue.value)
  if (isNaN(value)) {
    alert('Please enter a valid number')
    return
  }

  count.value -= value
}

const submitHandler = (event) => {
  event.preventDefault()

  const value = Number(event.target[0].value)
  if (isNaN(value)) {
    alert('Please enter a valid number')
    return
  }

  if (increment) {
    count.value += value
  }

  if (decrement) {
    count.value -= value
  }
}
</script>

<template>
  <div class="eventButtons">
    <form @:submit="submitHandler">
      <input v-model="inputValue" type="text" placeholder="Enter a number" class="global-box" />
      <button @:click="increment" class="global-box increment-button">Increment</button>
      <button @:click="decrement" class="global-box increment-button">Decrement</button>
    </form>
  </div>
  <h1>Count: {{ count }}</h1>
</template>

<style>
.eventButtons {
  display: flex;
  justify-content: space-around;
  gap: 1rem;
  width: 95%;
}

.increment-button {
  border: 0;
  background-color: hsl(160, 100%, 37%);
  color: white;
  font-size: 1.5rem;
}
</style>
