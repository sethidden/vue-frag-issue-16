<template>
<div v-frag v-if="visible" data-id153="i-am-myinput-root">
    <div>
      I'm an input
    </div>
  </div>
</template>

<script>
import frag from 'vue-frag'
export default {
  props: ['visible'], directives: {frag}}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
