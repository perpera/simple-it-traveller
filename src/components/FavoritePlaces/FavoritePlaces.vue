<script setup>
import FavoritePlace from '../FavoritePlace/FavoritePlace.vue'
import IButton from '../IButton/IButton.vue'
</script>

<template>
  <div class="px-6">
    <div class="text-gray mb-4">Added Pins</div>
    <slot name="label"></slot>
    <slot name="list"><FavoritePlace :key="n" v-for="n in 4" /></slot>
    <slot></slot>
    <IButton class="w-full mt-10"> Add pin</IButton>
  </div>
</template>
