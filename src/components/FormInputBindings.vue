<script setup lang="ts">
import { ref } from 'vue'

const options = ['option1', 'option2', 'option3']

const text = ref('')
const checobox = ref(false)
const radio = ref(options[0])
const select = ref(options[0])
const checkboxes = ref([])
</script>

<template>
  <h1>Form Input Bindings</h1>

  <section>
    <h2>Text</h2>
    <input v-model="text" />
    <p>Text: {{ text }}</p>
  </section>

  <section>
    <h2>Checkbox</h2>
    <input type="checkbox" v-model="checobox"/>
    <p>Checkbox: {{ checobox ? 'TRUE' : 'FALSE' }}</p>
  </section>

  <section>
    <h2>Radio</h2>
    <label v-for="option in options">
      <input type="radio" :value="option" v-model="radio">
      {{ option }}
    </label>
    <p>Radio: {{ radio }}</p>
  </section>

  <section>
    <h2>Select</h2>
    <select v-model="select">
      <option v-for="option in options" :value="option">
        {{ option }}
      </option>
    </select>
    <p>Select: {{ select }}</p>
  </section>

  <section>
    <h2>Multiple Checkbox</h2>
    <label v-for="option in options">
      <input type="checkbox" :value="option" v-model="checkboxes">
      {{ option }}
    </label>
    <p>Multiple Checkbox: {{ checkboxes }}</p>
  </section>
</template>
