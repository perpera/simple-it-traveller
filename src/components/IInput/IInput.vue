<script setup>
const props = defineProps({
  label: String,
  placeholder: String,
  type: {
    default: 'text',
    type: String,
  },
})

defineOptions({
  inheritAttrs: false,
})
</script>

<template>
  <div class="w-full text-[#2c2c2c]">
    <label class="block">
      <span class="block text-xs px-3 mb-2">{{ props.label }}: {{ text }}</span>
      <input
        class="w-full text-sm rounded-[4px] border-[#eaeaea] border-[1px] py-2 px-3 focus:outline-primary"
        v-bind="{ ...$props, ...$attrs }"
        @input="changeValue"
      />
    </label>
  </div>
</template>
