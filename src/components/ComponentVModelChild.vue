<script setup lang="ts">
const model = defineModel({ default: 0 })
</script>

<template>
  <button @click="() => model++">Count Up</button>
  <p>v-model: {{ model }}</p>
</template>
