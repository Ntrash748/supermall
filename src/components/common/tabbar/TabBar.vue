<template>
  <div class="tab-bar">
    <slot></slot>
  </div>
</template>
<script>
export default {
  name: 'TabBar'
}
</script>
<style scoped>
  .tab-bar {
    display: flex;
    text-align: center;
    height: 48px;
    position: fixed;
    left: 0;
    right: 0;
    bottom: 0;
    background-color: #f6f6f6;
    box-shadow: 0 -1px 1px rgba(100, 100, 100, .1);
    z-index: 10;
  }
</style>