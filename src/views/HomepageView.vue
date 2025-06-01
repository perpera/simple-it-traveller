<script setup>
import IButton from '../components/IButton/IButton.vue'
</script>

<template>
  <main class="flex h-screen">
    <section class="flex-1 flex justify-center items-center bg-primary">
      <div class="text-center text-white px-8">
        <img class="inline mb-6" src="../assets//img/map-pin.svg" alt="map-pin icon" />
        <h1 class="font-bold text-[38px] mb-7">IT traveler</h1>
        <p class="leading-6 mb-11">
          A simple and convenient web application that will let you mark your favourite places, as
          well as those you would really like to visit. So don't hesitate and try it out yourself.
        </p>
        <IButton>Get started</IButton>
      </div>
    </section>
    <section class="flex-1">
      <img class="h-full object-cover w-full" src="../assets/img/map.png" alt="preview map" />
    </section>
  </main>
</template>
