<script setup lang="ts">
import ComponentProvideInjectChild from './ComponentProvideInjectChild.vue'

import { provide, ref } from 'vue'

const count = ref(0)
function countUp() {
  count.value++
}
provide('count', { count, countUp })
</script>

<template>
  <h1>Component Provide / Inject</h1>

  <section>
    <ComponentProvideInjectChild />
  </section>
</template>
