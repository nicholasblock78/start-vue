<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Money />
    <h1>hello</h1>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Money from './components/Money.vue'

export default {
  name: 'app',
  components: {
    Money,
    HelloWorld
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
