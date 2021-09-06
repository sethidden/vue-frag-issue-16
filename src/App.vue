<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <MyInput :visible="toggler2" />
    <MyInput :visible="toggler2" />
    <MyInput :visible="toggler" />
  </div>
</template>

<script>
import frag from 'vue-frag'
import MyInput from './MyInput.vue'
export default {
  components: { MyInput },
  name: 'App',
  directives: {
    frag 
  },
  data() {
    return {
      toggler: false,
      toggler2: true,
    }
  },
  mounted() {
    setInterval(() => {this.toggler = !this.toggler; this.toggler2 = !this.toggler2}, 1)
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
