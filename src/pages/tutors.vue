<script setup lang="ts">
import { NButton } from '@nethren-ui/vue'
import PageHeading from '~/components/common/PageHeading.vue'
import Tutor from '~/components/Tutor.vue'
</script>

<template>
  <div class="tutors-page">
    <header class="flex justify-end h-[60px] items-center">
      <!-- <img :src="logo" alt="" class="w-[9rem] h-[3rem] px-3 pt-3"> -->
      <div class="flex gap-8 px-6 pt-4 items-center">
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="/tutors">Tutors</a>
        <a href="#">Classes</a>
        <a href="#">Contact Us</a>
        <NButton mode="solid">
          Login
        </NButton>
      </div>
    </header>
  </div>

  <PageHeading class="text-center mt-2">
    Our Tutors
  </PageHeading>

  <div>
    <p class="font-semibold text-xl px-[6rem]">
      Science/ Maths
    </p>
    <div class="tutors">
      <Tutor
        :details="{ name: 'Ruwan Darshana', class: 'Combined Mathematics', image: '/ruwan-darshana.jpg' }"
      />

      <Tutor
        :details="{ name: 'Nilantha Jayasuriya', class: 'Physics', image: '/nilantha-jayasuriya.jpg' }"
      />

      <Tutor
        :details="{ name: 'Janaka Abewansha', class: 'Chemistry', image: '/janaka-abewansha.jpg' }"
      />

      <Tutor
        :details="{ name: 'Hiranga Sovis', class: 'Chemistry', image: '/hiranga.jpg' }"
      />

      <Tutor
        :details="{ name: 'Nirandika Jayawardhana', class: 'Chemistry', image: '/nirandika.jpg' }"
      />
    </div>
  </div>

  <div>
    <p class="font-semibold text-xl px-[6rem] mt-[1rem]">
      Commerce
    </p>

    <div class="tutors ">
      <Tutor
        :details="{ name: 'Amaranath Batagoda', class: 'Economics', image: '/amranath_batagoda.jpg' }"
      />

      <Tutor
        :details="{ name: 'Gayan Sampath', class: 'Business Studies', image: '/gayan-sampath.png' }"
      />

      <Tutor
        :details="{ name: 'Chaminda Vidanage', class: 'Accounting', image: '/chaminda-vidanage.jpg' }"
      />
    </div>
  </div>

  <div>
    <p class="font-semibold text-xl px-[6rem] mt-[1rem]">
      Technology
    </p>

    <div class="tutors ">
      <Tutor
        :details="{ name: 'Dananjaya Kalugampitiya', class: 'ICT', image: '/dananjaya-kalugampitiya.jpg' }"
      />

      <Tutor
        :details="{ name: 'Dinesh Athukorala', class: 'BST', image: '/dinesh-athukorala.jpg' }"
      />

      <Tutor
        :details="{ name: 'Chamara Sanjeewa', class: 'SFT', image: '/chamara-sir.jpg' }"
      />

      <Tutor
        :details="{ name: 'Sanjeewa Wijesiri', class: 'SFT', image: '/sanjeewaWijesiri.jpg' }"
      />
    </div>
  </div>

  <div>
    <p class="font-semibold text-xl px-[6rem] mt-[1rem]">
      Art
    </p>

    <div class="tutors ">
      <Tutor
        :details="{ name: 'Danushka Vithanage', class: 'Media', image: '/dhanushka-vithanage.jpg' }"
      />

      <Tutor
        :details="{ name: 'Nishshanka Rajaguru', class: 'SFT', image: '/nishshanka-rajaguru.jpg' }"
      />
    </div>
  </div>

  <div>
    <p class="font-semibold text-xl px-[6rem] mt-[1rem]">
      Common
    </p>

    <div class="tutors ">
      <Tutor
        :details="{ name: 'Madusanka Samarakoon', class: 'General English', image: '/madusanka-samarakoon.jpg' }"
      />
    </div>
  </div>
</template>

<style scoped lang="scss">
.tutors{
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    grid-template-rows: repeat(1, 300px);
    padding-block: 1rem;
    padding-inline: 4rem;
    gap: 1rem;
    justify-content: space-between;
}
</style>
