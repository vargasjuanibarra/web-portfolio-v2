<template>
  <div class="flex flex-col items-center md:py-12 lg:py-24 w-full">
    <h3 class="text-2xl font-semibold md:text-4xl lg:text-5xl text-white pb-12">Professional <span class="text-emerald-400">experiences</span></h3>
    <div class="relative flex flex-col">
      <div 
        v-for="(event, index) in events" 
        :key="index" 
        :class="'flex w-full after:absolute after:hidden md:after:block after:w-1 after:h-full after:bg-slate-50 after:top-0 after:left-0 after:z-[50] md:after:left-1/2 ' + (index % 2 === 0 ? 'justify-start' : 'justify-end')"
      >
      <div class="px-2 py-4 md:px-8 md:w-1/2 lg:px-8 md:py-8 hover:-translate-y-4 duration-200 z-[100]">
        <div class="relative p-4 shadow-xl bg-slate-50 rounded-lg">
          <div :class="'hidden md:block bg-slate-400 rounded-full w-12 h-12 absolute z-[100] top-0 ' + (index % 2 === 0 ? '-right-14' : '-left-14')">
            <div class="relative shadow-lg grid place-items-center ">
              <img :src="event.img" class="object-cover text-2xl font-bold text-black w-full h-full rounded-full"/>
            </div>
          </div>
          <h3 class="mb-1 font-bold text-gray-800 text-lg md:text-xl">{{ event.title }}</h3>
          <p class="leading-tight text-justify text-gray-700">{{ event.description }}</p>
          <span class="text-gray-500 text-sm">{{ event.date }}</span>
        </div>
      </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import suitespotImg from '../assets/suitespot.png';
import crewbloomImg from '../assets/crewbloom.webp';
import adriotdevImg from '../assets/adriot.png';

const events = [
  { title: 'Fullstack Developer at Suitespot Inc.', description: 'I blend creativity and analytical rigor to design and implement robust front-end interfaces and scalable back-end systems. My work focuses on developing innovative solutions that elevate user experiences and ensure seamless application performance.', date: 'Aug 2022 - July 2024', img: suitespotImg },
  { title: 'Web Developer at Crewbloom', description: 'As a Junior Web Developer at CrewBloom, I focus on developing and maintaining dynamic web applications. My work involves collaborating with cross-functional teams to ensure seamless user experiences, implementing responsive design principles, and optimizing performance to deliver high-quality digital solutions.', date: 'June 2021 - April 2022', img: crewbloomImg },
  { title: 'Junior Developer at AdRiot Dev', description: 'I work on building and optimizing web applications. My responsibilities include implementing responsive designs, enhancing user interfaces, and collaborating with teams to deliver seamless digital experiences. I focus on ensuring performance and usability while contributing to innovative web solutions.', date: 'March 2021 - June 2021', img:adriotdevImg },
  // Add more events as needed
];
</script>

<style>
/* Additional styles if necessary */
</style>
