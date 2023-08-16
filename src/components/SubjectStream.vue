<script setup lang="ts">
import type { SubjectDetails } from '~/types'

interface SubjectDetailsProps {
  details: SubjectDetails
}

defineProps<SubjectDetailsProps>()
</script>

<template>
  <div
    class="mt-0.5 flex text-white flex items-center justify-center" style="box-shadow: 0 0.25rem 1rem rgba(0, 0, 0, 0.1);"
    :style="{
      backgroundImage: `linear-gradient(to left, rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.3)), url(${details.image})`,
      backgroundColor: 'rgba(0, 0, 0, 0.6)',
      backgroundRepeat: 'no-repeat',
      backgroundSize: 'cover',
      backgroundPosition: 'center',
      backgroundImageHeight: '4rem',
      borderRadius: '0.5rem',
    }"
  >
    <p class="text-3xl font-semibold flex items-center justify-center">
      {{ details.name }}
    </p>
  </div>
</template>

<style scoped lang="scss">
// .subject-image .foreground{
//     background-color: rgba(0, 0, 0, 0);
//     border-radius: 1rem;
//     width: 100%;
//     height: 100%;
//     display: flex;
//     flex-direction: column;
//     align-items: center;
//     justify-content: flex-start;
//     transition: all 0.3s ease-in-out;

// }
</style>
