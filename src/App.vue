<template>
<NavBarComp></NavBarComp>
<ContainerComp></ContainerComp>
</template>

<script lang="js">

import NavBarComp from './components/NavBarComp.vue'
import ContainerComp from './components/ContainerComp.vue'
export default {
  name: 'App',
  components: {
    NavBarComp,ContainerComp
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0;
}
</style>
