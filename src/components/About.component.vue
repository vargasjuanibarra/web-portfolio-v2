<template>
  <div class="md:mt-12 md:py-8">
    <div class="pb-12" id="highlight">
      <div
        class="mb-8 flex flex-col gap-2 text-center text-white relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-slate-50 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-slate-50 py-4"
      >
        <p class="text-2xl font-semibold md:text-4xl lg:text-5xl">
          Meet the <span class="text-emerald-400">Developer</span>
        </p>
      </div>
    </div>
    <div
      v-for="(item, index) in aboutSection"
      :key="index"
      class="max-w-[500px] py-4 flex p-4 gap-6 mx-auto sm:max-w-[600px] lg:max-w-[800px] text-white"
    >
      <h3 class="hidden sm:block text-2xl md:text-4xl lg:text-5xl font-bold">
        {{ item.category }}
      </h3>
      <div class="flex flex-col justify-start">
        <span class="text-2xl md:text-4xl lg:text-5xl font-normal">{{
          item.label
        }}</span>
        <p
          class="text-md md:text-lg lg:text-xl font-normal text-wrap py-4 text-justify"
        >
          {{ item.description }}
        </p>
      </div>
    </div>
  </div>
</template>
<script setup>
const aboutSection = [
  {
    id: 1,
    category: 'I',
    label: 'a self taught developer',
    description:
      'I learned to code through online resources, discovering a passion for the creative problem-solving inherent in crafting innovative digital experiences. Beginning with JavaScript, HTML & CSS, I expanded into frameworks, backend development, design, and much much more.',
  },
  {
    id: 2,
    category: 'II',
    label: 'obsessed with perfecting product design and UX',
    description:
      'With an insatiable curiosity for product design and UX, I approach each project with a blend of creativity and analytical rigor, seeking to uncover innovative solutions that elevate the user experience to new heights.',
  },
  {
    id: 3,
    category: 'III',
    label: 'valued team player and dedicated contributor',
    description:
      "As a team player and contributor, I thrive on collaboration and cooperation, valuing the collective effort over individual achievement. I actively engage with my colleagues, offering support, sharing ideas, and leveraging diverse perspectives to achieve shared goals. With a strong commitment to teamwork, I strive to foster a positive environment where everyone's contributions are valued and respected, ultimately driving the team towards success.",
  },
];
</script>
<style lang=""></style>
