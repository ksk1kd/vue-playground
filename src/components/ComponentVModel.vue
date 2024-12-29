<script setup lang="ts">
import ComponentVModelChild from './ComponentVModelChild.vue'

import { ref } from 'vue'
const count = ref(10)
</script>

<template>
  <h1>Component v-model</h1>

  <section>
    <ComponentVModelChild v-model="count"/>
  </section>
</template>
