<script setup lang="ts">
import { NButton } from '@nethren-ui/vue'
import logo from '~/assets/images/logo.png'
import landing from '~/assets/images/landing.png'
import StudentThought from '~/components/StudentThought.vue'
import SubjectStream from '~/components/SubjectStream.vue'
import map from '~/assets/images/map.jpg'
</script>

<template>
  <div class="landing-page">
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

    <div class="bg-var(--n-color-primary-400) flex items-center w-[100%] pl-15 pr-4 my-4 h-[calc(100vh)]">
      <div class="flex flex-col items-center justify-center w-[65%]">
        <img :src="logo" alt="" class=" px-3 pt-3">

        <h1 class="font-bold text-4xl text-[#230D79] text-left ml-[2rem]">
          Experimental and Experienced Learning
        </h1>

        <div class="my-10 px-3 flex justify-start self-start ml-[2rem]">
          <NButton mode="solid" class="" style="padding-inline: 5rem; padding-block: 1.5rem;">
            Get Started
          </NButton>
        </div>
      </div>

      <img :src="landing" alt="" class="w-[60%]">
    </div>

    <div class="bg-[var(--n-color-primary-400)] text-center">
      <p class="font-semibold text-xl py-6 text-white">
        Join 2024 A/L Classes Live or Physical
      </p>
    </div>

    <div class="landing-container my-6 ">
      <SubjectStream :details="{ name: 'Science/Maths', image: '/science.jpg' }" class="science-container" />
      <SubjectStream :details="{ name: 'Arts', image: '/art.jpg' }" class="arts-container" />
      <SubjectStream :details="{ name: 'Commerce', image: '/commerce.jpg' }" class="commerce-container" />
      <SubjectStream :details="{ name: 'Technology', image: '/tech.jpg' }" class="tech-container" />
      <SubjectStream :details="{ name: 'Live Classes', image: '/live.jpg' }" class="live-container" />
    </div>

    <div class="bg-[var(--n-color-primary-400)] justify-between flex p-8">
      <div class="flex flex-col gap-2">
        <p class="font-semibold text-4xl text-white text-center">
          3000+
        </p>
        <p class="font-semibold text-white text-center">
          Students
        </p>
      </div>

      <div class="flex flex-col gap-2">
        <p class="font-semibold text-4xl text-white text-center">
          3000+
        </p>
        <p class="font-semibold text-white text-center">
          Students
        </p>
      </div>

      <div class="flex flex-col gap-2">
        <p class="font-semibold text-4xl text-white text-center">
          3000+
        </p>
        <p class="font-semibold text-white text-center">
          Students
        </p>
      </div>

      <div class="flex flex-col gap-2">
        <p class="font-semibold text-4xl text-white text-center">
          3000+
        </p>
        <p class="font-semibold text-white text-center">
          Students
        </p>
      </div>

      <div class="flex flex-col gap-2">
        <p class="font-semibold text-4xl text-white text-center">
          3000+
        </p>
        <p class="font-semibold text-white text-center">
          Students
        </p>
      </div>
    </div>

    <div>
      <div class="flex gap-36 py-4 px-20 my-8 text-justify w-[90%]" style="margin-inline: auto;">
        <div>
          <p class="text-4xl font-semibold my-8 flex flex-col justify-center items-center text-[#230D79]">
            More about our academy
          </p>
          <p>
            We are proud to present your door to becoming a first-time qualified higher education student in Nugegoda.
            "Sailing Pen Academy of Higher Education" is a luxury, high-tech and modern technology auditorium for prospective
            children.
          </p> <br>
          <p>
            The Higher Education Academy features indoor and outdoor air-conditioned auditoriums, sophisticated speakers,
            lecture facilities such as widescreen features and clean, comfortable seating arrangements and a cafeteria with a
            pleasing surrounding.
          </p>
        </div>

        <img src="/info.jpg" alt="" class="w-[50%] rounded-xl">
      </div>
    </div>

    <div class="bg-[var(--bg-primary)] py-4">
      <p class="text-4xl font-semibold mt-4 text-[#230D79] text-center">
        Online Class Features
      </p>
      <div class="features">
        <div class="text-center ">
          <div class="flex gap-8 justify-center">
            <p class="text-2xl font-semibold text-[var(--n-color-primary-400)] mb-5">
              Lesson Packs
            </p>
            <game-icons-bookshelf class="text-[var(--n-color-primary-400)] text-2xl" />
          </div>

          <p class="text-justify">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Incidunt ratione excepturi placeat quos ullam doloremque sequi
            fugiat accusantium, veritatis alias. Ut minus harum placeat maiores aliquid. Vel magni saepe ab!
          </p>
        </div>

        <div>
          <div class="flex gap-8 justify-center">
            <p class="text-2xl font-semibold text-[var(--n-color-primary-400)] mb-5 text-center">
              Classes
            </p>
            <mdi-google-classroom class="text-[var(--n-color-primary-400)] text-2xl" />
          </div>

          <p class="text-justify">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Incidunt ratione excepturi placeat quos ullam doloremque sequi
            fugiat accusantium, veritatis alias. Ut minus harum placeat maiores aliquid. Vel magni saepe ab!
          </p>
        </div>

        <div>
          <div class="flex gap-8 justify-center">
            <p class="text-2xl font-semibold text-[var(--n-color-primary-400)] mb-5 text-center">
              Exams
            </p>
            <healthicons-i-exam-qualification class="text-[var(--n-color-primary-400)] text-2xl" />
          </div>

          <p class="text-justify">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Incidunt ratione excepturi placeat quos ullam doloremque sequi
            fugiat accusantium, veritatis alias. Ut minus harum placeat maiores aliquid. Vel magni saepe ab!
          </p>
        </div>

        <div>
          <div class="flex gap-8 justify-center">
            <p class="text-2xl font-semibold text-[var(--n-color-primary-400)] mb-5 text-center">
              Quizzes
            </p>
            <ic-twotone-quiz class="text-[var(--n-color-primary-400)] text-2xl" />
          </div>

          <p class="text-justify">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Incidunt ratione excepturi placeat quos ullam doloremque sequi
            fugiat accusantium, veritatis alias. Ut minus harum placeat maiores aliquid. Vel magni saepe ab!
          </p>
        </div>

        <div>
          <div class="flex gap-8 justify-center">
            <p class="text-2xl font-semibold text-[var(--n-color-primary-400)] mb-5 text-center">
              Leader Board
            </p>
            <material-symbols-social-leaderboard-outline-rounded class="text-[var(--n-color-primary-400)] text-2xl" />
          </div>

          <p class="text-justify">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Incidunt ratione excepturi placeat quos ullam doloremque sequi
            fugiat accusantium, veritatis alias. Ut minus harum placeat maiores aliquid. Vel magni saepe ab!
          </p>
        </div>

        <div>
          <div class="flex gap-8 justify-center">
            <p class="text-2xl font-semibold text-[var(--n-color-primary-400)] mb-5 text-center">
              Flash Cards
            </p>
            <mdi-cards class="text-[var(--n-color-primary-400)] text-2xl" />
          </div>

          <p class="text-justify">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Incidunt ratione excepturi placeat quos ullam doloremque sequi
            fugiat accusantium, veritatis alias. Ut minus harum placeat maiores aliquid. Vel magni saepe ab!
          </p>
        </div>
      </div>
    </div>

    <div>
      <p class="text-4xl font-semibold my-8 text-[#230D79] text-center">
        Students' Thought
      </p>
      <div class="student-thought">
        <StudentThought
          :details="{ profilePicture: '/student-profile-2.jpg', name: 'Amani Vidanage', class: '2023 A/L Commerce', thought: 'As a college-level commerce student at SailingPen Academy, I feel fortunate to have the opportunity to refine my business acumen through their advanced courses. The academy commitment to providing a comprehensive understanding of commerce and economics, along with practical exposure to real-world scenarios, is what drew me here. I am eager to engage in discussions with industry experts and fellow students, as well as to explore case studies that bridge the gap between theory and practice.' }"
        />

        <StudentThought
          :details="{ profilePicture: '/student-profile.jpg', name: 'Ishini Avindya', class: '2023 A/L Science', thought: 'I am really excited to be a part of SailingPen Academy science program. The academy is reputation for offering advanced-level courses in various streams is impressive, and I can not wait to dive into challenging subjects like physics, chemistry, and biology. The hands-on approach to learning and the availability of state-of-the-art laboratory facilities are particularly appealing to me. I am looking forward to expanding my scientific horizons and preparing myself for a future in research or academia.' }"
        />

        <StudentThought
          :details="{ profilePicture: '/student-profile-3.jpg', name: 'Randima Dias', class: '2020 A/L Arts', thought: 'SailingPen Academy unique blend of art and technology education is exactly what I have been searching for. As a student passionate about both creative expression and innovative technology, I am thrilled to join their program. The academy emphasis on interdisciplinary learning will allow me to explore the intersections between art and technology, and their advanced level curriculum promises to challenge me in ways that traditional art schools might not. With access to cuttingedge software and equipment.' }"
        />
      </div>
    </div>

    <div class="bg-[var(--bg-primary)] pt-4">
      <p class="text-4xl font-semibold my-8 text-[#230D79] text-center">
        Life at SailingPen
      </p>
      <div class="life-grid px-18">
        <img src="/life1.jpg" alt="" class="image1 w-[100%] h-[100%]">
        <img src="/life2.jpg" alt="" class="image2 w-[100%] h-[100%]">
        <img src="/life3.jpg" alt="" class="image3 w-[100%] h-[100%]">
        <img src="/life4.jpg" alt="" class="image4 w-[100%] h-[100%]">
        <img src="/life5.jpg" alt="" class="image5 w-[100%] h-[100%]">
      </div>
    </div>

    <div class="bg-[#282A3A] p-8 text-white ">
      <div class="flex gap-41">
        <div class="text-center flex flex-col justify-center">
          <div class="flex gap-2 items-center mb-2">
            <material-symbols-call class="text-white" />
            <p class="font-semibold">
              Contact Us
            </p>
          </div>

          <p>011 2810061</p>
          <p>075 5882882</p>
          <p>070 6767502</p>
          <p>070 6767503</p>
          <p>070 6767505</p>
          <p>070 6767506</p>
        </div>

        <div class="flex gap-2 items-center">
          <material-symbols-location-on-rounded class="text-white" />
          <p>24, Papiliyana Rd, Gangodavila, Nugegoda</p>
        </div>

        <div class="flex gap-2 items-center">
          <ic-baseline-mail class="text-white" />
          <p>contact@sailingpen.com</p>
        </div>

        <img :src="map" alt="" class="w-[22%] h-[20%]">
      </div>
      <p class="text-center">
        Copyright © 2023 SailingPen | All rights reserved. | Powerd by EduRa
      </p>
    </div>
  </div>
</template>

<style scoped lang="scss">
.landing-container{
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(2, 300px);
    grid-template-areas:
        "science live arts"
        "commerce live tech";
    gap: 3rem;
    padding-inline: 3rem;
}

.science-container{
    height: 100%;
    grid-area: science;
}

.live-container{
    height: 100%;
    grid-area: live;
}

.arts-container{
    height: 100%;
    grid-area: arts;
}

.commerce-container{
    height: 100%;
    grid-area: commerce;
}

.tech-container{
    height: 100%;
    grid-area: tech;
}

.features{
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 6rem;
    padding: 3rem 8rem;
}

.student-thought{
    display: grid;
    grid-template-columns: repeat((3, 1fr));
    gap: 5rem;
    padding: 1rem 6rem;
}

.life-grid{
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-areas:
        "image1 image2 image3"
        "image4 image2 image5";
}

.image1{
    grid-area: image1;
}

.image2{
    grid-area: image2;
}

.image3{
    grid-area: image3;
}

.image4{
    grid-area: image4;
}

.image5{
    grid-area: image5;
}
</style>
