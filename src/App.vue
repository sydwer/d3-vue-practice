<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Chart />
  </div>
</template>

<script>
import * as d3 from 'd3'

import HelloWorld from './components/HelloWorld.vue'
import Chart from './components/Chart.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Chart
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
