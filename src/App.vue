<script setup lang="ts">
import ComponentProps from './components/ComponentProps.vue'
import ComputedProperties from './components/ComputedProperties.vue'
import FormInputBindings from './components/FormInputBindings.vue'
</script>

<template>
  <div class="container">
    <ComputedProperties />
    <ComponentProps stringProp="aaa" :numberProp="Number(100)" :booleanProp="true" :arrayProp="['aaa', 'bbb']"/>
    <FormInputBindings />
  </div>
</template>

<style scoped>
.container {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
}
</style>
