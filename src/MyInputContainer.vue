<template>
  <MyFragment data-id2="i-am-my-input-container-root">
    <slot name="label" />
    <div>
      <slot />
    </div>
  </MyFragment>
</template>

<script lang="ts">
import MyFragment from './MyFragment.vue';

export default {components: { MyFragment } };
</script>
