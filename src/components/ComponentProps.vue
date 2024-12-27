<script setup lang="ts">
interface Props {
  stringProp: string
  numberProp: number
  booleanProp: boolean
  arrayProp: string[]
}

const { stringProp, numberProp, booleanProp, arrayProp } = defineProps<Props>()
</script>

<template>
  <h1>Component Props</h1>

  <section>
    <p>stringProp: {{ stringProp }}</p>
    <p>numberProp: {{ numberProp }}</p>
    <p>booleanProps: {{ booleanProp }}</p>
    <p>arrayProps: {{ arrayProp }}</p>
  </section>
</template>
