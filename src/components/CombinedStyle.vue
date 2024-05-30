<template>
  <h2 class="g-1">Another Global Style</h2>
  <h2 class="l-1">Another Local Style</h2>
</template>

<style>
.g-1 {
  background: hsla(160, 100%, 37%, 1);
  width: 95%;
  padding: 1rem 1rem;
  margin: 1rem 0;
  border-radius: 5px;
  color: white;
}
</style>

<style scoped>
.l-1 {
  color: hsla(160, 100%, 37%, 1);
  /* width: 95%; */
  padding: 1rem 1rem;
  margin: 1rem 0;
  border-radius: 5px;
}
</style>
