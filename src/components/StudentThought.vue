<script setup lang="ts">
import type { StudentThoughtDetails } from '~/types/'

interface StudentThoughtProps {
  details: StudentThoughtDetails
}

defineProps<StudentThoughtProps>()
</script>

<template>
  <div>
    <div class="flex gap-4 items-center justify-center">
      <img :src="details.profilePicture" alt="" class="w-[50px] h-[50px]" style="aspect-ratio: 1; border-radius: 50%;">
      <div>
        <p class="font-semibold">
          {{ details.name }}
        </p>
        <p class="font-semibold">
          {{ details.class }}
        </p>
      </div>
    </div>
    <p class="mt-6 text-justify">
      {{ details.thought }}
    </p>
  </div>
</template>
