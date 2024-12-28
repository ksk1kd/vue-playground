<script setup lang="ts">
import { computed, ref } from 'vue'

const firstName = ref('John')
const lastName = ref('Doe')

const fullName = computed(() => `${firstName.value} ${lastName.value}`)
</script>

<template>
  <h1>Computed Properties</h1>

  <section>
    <label>
      First Name: 
      <input type="text" v-model="firstName">
    </label>
    <label>
      Last Name: 
      <input type="text" v-model="lastName">
    </label>
    <p>Full Name: {{ fullName }}</p>
  </section>
</template>
