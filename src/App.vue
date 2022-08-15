<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <BaseContainer msg="Welcome to Your Vue.js App"/>
</template>

<script>
import BaseContainer from './components/BaseContainer.vue'

export default {
  name: 'App',
  components: {
    BaseContainer,
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
  margin-top: 60px;
}
</style>
