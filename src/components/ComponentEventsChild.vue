<script setup lang="ts">
interface Props {
  eventName: string
}

interface Emits {
  someEvent: []
}

const { eventName } = defineProps<Props>()
const emit = defineEmits<Emits>()
</script>

<template>
  <button @click="emit('someEvent')">{{ eventName }}</button>
</template>
