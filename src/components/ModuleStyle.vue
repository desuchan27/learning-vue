<script>
import './GlobalStyle.vue'
</script>

<template>
  <h2 :class="[$style['m-class'], 'global-box']">Using Module CSS with $ syntax (kabak-case)</h2>
  <h2 :class="[$style.camelCaseClass, 'global-box']">Using Module CSS with $ syntax</h2>
</template>

<style module>
/* kebak */
.m-class {
  background-color: white;
  color: hsl(160, 100%, 37%);
  width: 95%;
  /* padding: 1rem 1rem;
  margin-bottom: 1rem;
  border-radius: 5px; */
}

.camelCaseClass {
  color: white;
  /* padding: 1rem 1rem;
  margin-bottom: 1rem;
  border-radius: 5px; */
}
</style>

<style module>
/* kebak */
.m-class {
  background-color: white;
  color: hsl(160, 100%, 37%);
  width: 95%;
  /* padding: 1rem 1rem;
  margin-bottom: 1rem;
  border-radius: 5px; */
}

.camelCaseClass {
  color: white;
  /* padding: 1rem 1rem;
  margin-bottom: 1rem;
  border-radius: 5px; */
}
</style>
