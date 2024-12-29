<script setup lang="ts">
defineOptions({
  inheritAttrs: false,
})
</script>

<template>
  <div class="child-wrapper">
    <button class="child" v-bind="$attrs">Click here!</button>
  </div>
</template>
