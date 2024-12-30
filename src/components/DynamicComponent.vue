<script setup lang="ts">
import DynamicComponentChildA from './DynamicComponentChildA.vue'
import DynamicComponentChildB from './DynamicComponentChildB.vue'

import { ref } from 'vue'
const currentTab = ref<'A' | 'B'>('A')
const tabs = {
  A: DynamicComponentChildA,
  B: DynamicComponentChildB,
}
</script>

<template>
  <h1>DynamicComponent</h1>

  <section>
    <ul>
      <li v-for="(_, tab) in tabs" :key="tab">
        <label>
          <input type="radio" :value="tab" v-model="currentTab" />
          <span>{{ tab }}</span>
        </label>
      </li>
    </ul>
    <KeepAlive>
      <component :is="tabs[currentTab]"></component>
    </KeepAlive>
  </section>
</template>

<style>
ul {
  display: flex;
  gap: 20px;
  padding: 0;
  list-style: none;
}
</style>