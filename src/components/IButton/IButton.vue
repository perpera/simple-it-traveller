<script setup>
import { defineProps, computed } from 'vue'

const props = defineProps({
  variant: {
    default: 'primary',
    type: String,
    validator: (value) => {
      return ['primary', 'gradient', 'outlined'].includes(value)
    },
  },
})
const bgStyles = computed(() => {
  return props.variant === 'gradient'
    ? 'bg-gradient-to-r from-[#ffa279] to-[#f3743d]'
    : 'bg-[#ffa279]'
})
</script>

<template>
  <button class="rounded-xl py-[14px] px-10 text-white font-bold -tracking-wider" :class="bgStyles">
    <slot>Click me</slot>
  </button>
</template>
