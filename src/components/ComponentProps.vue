<script setup lang="ts">
import ComponentPropsChild from './ComponentPropsChild.vue'
</script>

<template>
  <h1>Component Props</h1>

  <section>
    <ComponentPropsChild stringProp="aaa" :numberProp="Number(100)" :booleanProp="true" :arrayProp="['aaa', 'bbb']"/>
  </section>
</template>
