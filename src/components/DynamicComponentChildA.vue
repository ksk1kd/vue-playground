<script setup lang="ts">
import { ref } from 'vue'
const text = ref('')
</script>

<template>
  <h2>Child A</h2>
  <input type="text" v-model="text">
</template>
