<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <vue-timeline :data="events"></vue-timeline>
  </div>
</template>

<script>
import VueTimeline from './components/VueTimeline.vue';
export default {
  name: 'App',
  components: {
    'vue-timeline': VueTimeline
  },
  data() {
    return {
      events: [{
          start: new Date(2021, 11,1),
          end: new Date(2021, 11,23),
          color: '#eee',
      },{
          name: "event 2",
          start: new Date(2021, 11,2),
          color: '#ff0000',
      },{
          name: "event 3",
          start: new Date(2021, 11,3),
          color: '#117700',
      },{
          name: "event 4",
          start: new Date(2021, 11,13),
          color: '#aa0099',
      },{
          name: "event 5",
          start: new Date(2021, 11,5),
          color: '#aa5599',
      }]
    }
  },
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
