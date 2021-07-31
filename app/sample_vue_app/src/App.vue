<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <!--<HelloWorld msg="Welcome to Your Vue.js App"/>-->
  <Sample1/>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import Sample1 from './components/Sample1.vue'
export default {
  name: 'App',
  components: {
    Sample1
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
