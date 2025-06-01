<script setup>
import FavIconButton from './FavIconButton.vue'
import DeleteIcon from './DeleteIcon.vue'
import EditIcon from './EditIcon.vue'
</script>

<template>
  <section class="text-gray mb-6 last:mb-0">
    <div class="flex gap-4">
      <img class="w-[76px] h-[76px] shrink-0" src="" alt="" />
      <div>
        <div class="flex justify-between items-center mb-2">
          <h2 class="font-bold text-[#2c2c2c]"></h2>
          <div class="flex gap-2">
            <FavIconButton>
              <EditIcon />
            </FavIconButton>
            <FavIconButton>
              <DeleteIcon />
            </FavIconButton>
          </div>
        </div>
        <p class="text-xs line-clamp-3"></p>
      </div>
    </div>

    <div class="h-[1px] w-full bg-[#ececec] mt-4"></div>
  </section>
</template>
