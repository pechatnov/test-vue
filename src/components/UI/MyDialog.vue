<template>
  <div v-if="show === true" class="dialog">
    <div class="dialog__content">
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: "my-dialog",
  props: {
    show: {
      type: Boolean,
      default: false,
    },
  },
};
</script>

<style scoped>
</style>