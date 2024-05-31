<template>
  <h1 class="text-red">Global Styling</h1>
  <p class="local">Trying local scope in this component</p>
</template>

<style>
.text-red {
  color: red;
}

.global-box {
  padding: 1rem 1rem;
  width: 95%;
  margin-bottom: 1rem;
  border-radius: 5px;
}

.increment-button {
  border: 0;
  background-color: hsl(160, 100%, 37%);
  color: white;
  font-size: 1.5rem;
}

.rows {
  display: flex;
  justify-content: space-around;
  gap: 1rem;
  width: 95%;
}
</style>
