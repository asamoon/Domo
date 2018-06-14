<template>
  <span :class="['badge', !!type ? 'badge--'+type : '']">
    <slot></slot>
  </span>
</template>

<script>
export default {
  name: 'badge',
  props: {
    type: {
      type: 'String',
      default: ''
    }
  }
}
</script>

<style lang="scss">
.badge {
  background: #999;
  display: inline-block;
  border-radius: .3rem;
  font-size: 1.2rem;
}
</style>
