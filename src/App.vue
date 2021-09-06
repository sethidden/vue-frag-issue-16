<template>
  <div id="app">
    <MyInput :visible="toggler" />
    <div v-if="toggler" />
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
    }
  },
  mounted() {
    setInterval(() => {this.toggler = !this.toggler;}, 500)
  }
}
</script>
