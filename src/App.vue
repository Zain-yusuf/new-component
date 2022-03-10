<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld />
    <parent  msg="Welcome zain how are you"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import parent from './components/parent.vue'
export default {
  name: 'App',
  components: {
    HelloWorld,
    parent
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
