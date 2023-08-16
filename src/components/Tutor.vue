<script setup lang="ts">
import type { TeacherDetails } from '~/types'

interface TeacherDetailsProps {
  details: TeacherDetails
}

defineProps<TeacherDetailsProps>()
</script>

<template>
  <div
    class="mt-0.5 flex text-white flex items-center justify-center" style="box-shadow: 0 0.25rem 1rem rgba(0, 0, 0, 0.1);"
    :style="{
      backgroundImage: `linear-gradient(to left, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0)), url(${details.image})`,
      backgroundColor: 'rgba(0, 0, 0, 0.6)',
      backgroundRepeat: 'no-repeat',
      backgroundSize: 'cover',
      backgroundPosition: 'center',
      backgroundImageHeight: '4rem',
      borderRadius: '0.5rem',
    }"
  >
    <div class="text-center flex flex-col mt-[14rem] bg-[rgba(0,0,0,0.5)] w-[16rem] py-[0.25rem] rounded-xl">
      <p class="font-semibold text-xl">
        {{ details.name }}
      </p>
      <p class="font-semibold">
        {{ details.class }}
      </p>
    </div>
  </div>
</template>
