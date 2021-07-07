<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import { removeWatermark, setWaterMark } from './common/water_mark'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  mounted() {
    setWaterMark('liergou', '李二狗');
},
destroyed() {
    removeWatermark();
},
}
</script>

<style>

</style>
