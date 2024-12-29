<script setup lang="ts">
import { inject } from 'vue'

const { count, countUp } = inject('count', {
  count: 0,
  countUp: () => {},
})
</script>

<template>
  <button @click="countUp">Count Up</button>
  <p>Count: {{ count }}</p>
</template>
