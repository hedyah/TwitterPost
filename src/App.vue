<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <TwitterContainer/>
  </div>
</template>

<script>

import TwitterContainer from './components/TwitterContainer.vue'
export default {
  name: 'App',
  components: {
    TwitterContainer
  }
}
</script>

<style>
*{
  background-color: cadetblue;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
