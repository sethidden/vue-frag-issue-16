<template>
  <div id="app">
    <div v-if="toggler" />
    <MyInput :visible="toggler" />
    <MyInput :visible="toggler2" />
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
      toggler2: false,
    }
  },
  mounted() {
    setInterval(() => {this.toggler = !this.toggler;}, 500)
    setInterval(() => {this.toggler2 = !this.toggler2;}, 250)
  }
}
</script>
