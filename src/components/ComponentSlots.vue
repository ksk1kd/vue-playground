<script setup lang="ts">
import ComponentSlotsChild from './ComponentSlotsChild.vue'
</script>

<template>
  <h1>Component Slots</h1>

  <section>
    <ComponentSlotsChild>
      <template #header>
        Card Header
      </template>

      <template #body>
      </template>
    </ComponentSlotsChild>
  </section>
</template>
