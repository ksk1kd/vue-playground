<script setup lang="ts">
import { ref, useTemplateRef } from 'vue'

const count = ref(0)
const input = useTemplateRef('input')

const countUp = () => {
  count.value++
}
</script>

<template>
  <h1>Event Handling</h1>

  <section>
    <h2>Click</h2>
    <button @click="countUp">Count Up</button>
    <p>count: {{ count }}</p>
  </section>

  <section>
    <h2>Key Modifier</h2>
    <p>Pressing the Enter key removes the focus from the input field.</p>
    <input ref="input" @keyup.enter="input?.blur" />
  </section>
</template>
