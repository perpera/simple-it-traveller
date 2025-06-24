<script setup>
import IInput from '../../IInput/IInput.vue'
import IButton from '../../IButton/IButton.vue'

const emit = defineEmits(['submit'])
</script>

<template>
  <form
    @submit.prevent="emit('submit', { name: 'Name' })"
    class="max-w-[500px] w-full bg-white p-10 rounded-[17px]"
  >
    <IInput class="mb-4" label="Full name" />
    <IInput class="mb-4" label="Email" placeholder="email@gmail.com" />
    <IInput label="Password" type="password" />
    <IButton class="mt-10 w-full" variant="gradient" type="submit">Create account</IButton>
  </form>
</template>
