<template>
  <div v-frag data-id3="i-am-my-fragment-root">
    <slot />
  </div>
</template>

<script>
import frag from 'vue-frag';
export default {
  directives: {
    frag,
  },
}
</script>
