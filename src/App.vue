<template>
 
  <NewComponent />
<Component2  title="Vuejs Tutorial" num="#1" modal="welcome..."/>
</template>


<script setup>
import NewComponent from './components/NewComponent.vue'
import Component2 from './Component2.vue'


</script>



<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
