<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Chart :data=data />
  </div>
</template>

<script>
// import * as d3 from 'd3'
// re-add in when fetching and using hooks to save the data etc.

import HelloWorld from './components/HelloWorld.vue'
import Chart from './components/Chart.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Chart
  },
  data(){
    return {
      data: {
        "tweets": [
          {"user": "Al", "content": "I really love seafood.", "timestamp": " Mon Dec 23 2013 21:30 GMT-0800 (PST)", "retweets": ["Raj","Pris","Roy"], "favorites": ["Sam"]},
          {"user": "Al", "content": "I take that back, this doesn't taste so good.", "timestamp": "Mon Dec 23 2013 21:55 GMT-0800 (PST)", "retweets": ["Roy"], "favorites": []},
          {"user": "Al", "content": "From now on, I'm only eating cheese sandwiches.", "timestamp": "Mon Dec 23 2013 22:22 GMT-0800 (PST)", "retweets": [], "favorites": ["Roy","Sam"]},
          {"user": "Roy", "content": "Great workout!", "timestamp": " Mon Dec 23 2013 7:20 GMT-0800 (PST)", "retweets": [], "favorites": []},
          {"user": "Roy", "content": "Spectacular oatmeal!", "timestamp": " Mon Dec 23 2013 7:23 GMT-0800 (PST)", "retweets": [], "favorites": []},
          {"user": "Roy", "content": "Amazing traffic!", "timestamp": " Mon Dec 23 2013 7:47  GMT-0800 (PST)", "retweets": [], "favorites": []},
          {"user": "Roy", "content": "Just got a ticket for texting and driving!", "timestamp": " Mon Dec 23 2013 8:05 GMT-0800 (PST)", "retweets": [], "favorites": ["Sam", "Sally", "Pris"]},
          {"user": "Pris", "content": "Going to have some boiled eggs.", "timestamp": " Mon Dec 23 2013 18:23 GMT-0800 (PST)", "retweets": [], "favorites": ["Sally"]},
          {"user": "Pris", "content": "Maybe practice some gymnastics.", "timestamp": " Mon Dec 23 2013 19:47  GMT-0800 (PST)", "retweets": [], "favorites": ["Sally"]},
          {"user": "Sam", "content": "@Roy Let's get lunch", "timestamp": " Mon Dec 23 2013 11:05 GMT-0800 (PST)", "retweets": ["Pris"], "favorites": ["Sally", "Pris"]}
        ]
}
    };
  },
};
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
