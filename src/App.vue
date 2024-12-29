<script setup lang="ts">
import ComponentEvents from './components/ComponentEvents.vue'
import ComponentProps from './components/ComponentProps.vue'
import ComputedProperties from './components/ComputedProperties.vue'
import EventHandling from './components/EventHandling.vue'
import FormInputBindings from './components/FormInputBindings.vue'
import Watchers from './components/Watchers.vue'
</script>

<template>
  <div class="container">
    <ComponentEvents />
    <ComponentProps />
    <EventHandling />
    <Watchers />
    <ComputedProperties />
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
