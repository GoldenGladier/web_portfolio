<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <Navigation />
    <Presentation />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Presentation from './components/Presentation.vue'
import Navigation from './components/Menu.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
    Presentation,
    Navigation
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
  /* margin-top: 60px; */
  margin: 0;
  padding: 0;
}
body{
  margin: 0;
  padding: 0;
}
</style>
