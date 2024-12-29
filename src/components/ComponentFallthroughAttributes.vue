<script setup lang="ts">
import ComponentFallthroughAttributesChild from './ComponentFallthroughAttributesChild.vue'
</script>

<template>
  <h1>Component Fallthrough Attributes</h1>

  <section>
    <ComponentFallthroughAttributesChild class="pass-class-from-parent" @click="() => console.log('Click here')"/>
  </section>
</template>
