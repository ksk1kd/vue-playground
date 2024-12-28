<script setup lang="ts">
import { ref, watch } from 'vue'

const text = ref('')
const errorMessage = ref('')

watch(text, (newText) => {
  if (newText.length >= 5) {
    errorMessage.value = "Don't over 5 characters."
  } else {
    errorMessage.value = ''
  }
})
</script>

<template>
  <h1>Watchers</h1>

  <section>
    <input type="text" v-model="text">
    <p v-show="errorMessage">{{ errorMessage }}</p>
  </section>
</template>
