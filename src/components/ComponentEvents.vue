<script setup lang="ts">
import ComponentEventsChild from './ComponentEventsChild.vue'

import { ref } from 'vue'
const count = ref(0)
</script>

<template>
  <h1>Component Events</h1>

  <section>
    <div>
      <ComponentEventsChild event-name="Count Up" @some-event="() => count += 1" />
    </div>
    <div>
      <ComponentEventsChild event-name="Count Up by 2" @some-event="() => count += 2" />
    </div>
    <p>Count: {{ count }}</p>
  </section>
</template>
