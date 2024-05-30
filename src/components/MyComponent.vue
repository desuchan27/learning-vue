<!-- JS -->
<script setup>
import NestedComponent from './NestedComponent.vue'

const name = 'Desu JS'
const imgInfo = {
  src: 'https://scontent.fceb6-1.fna.fbcdn.net/v/t39.30808-6/445229025_3720087498279070_8287430768663977059_n.jpg?_nc_cat=104&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeFCvPmyhswnH3edXNMzi3nx4s5oH1Qe5gzizmgfVB7mDKfDOYLH9MOjXslkTw9v3YXcc6qK3vLY7A87R8pTUkjM&_nc_ohc=iRMnJ1Qc-FgQ7kNvgHmSAol&_nc_ht=scontent.fceb6-1.fna&oh=00_AYCsNCZdssHkhFScfi9gLbFPqmlhxUQuBmXQve2Il9TWNg&oe=665D19DE',
  alt: "Desu's avatar"
}
</script>

<!-- HTML  -->
<template>
  <img :src="imgInfo.src" :alt="imgInfo.alt" />
  <div>
    <h1>{{ name }}</h1>
    <NestedComponent />
  </div>
</template>

<!-- CSS  -->
<style scoped>
h1 {
  font-weight: 900;
  color: #999;
}
img {
  width: 95%;
  border-radius: 1%;
  display: block;
  /* margin-right: 1rem; */
}
</style>
