<script setup lang="ts">
import { ref } from 'vue'
const text = ref('')
</script>

<template>
  <h2>Child B</h2>
  <input type="text" v-model="text">
</template>
