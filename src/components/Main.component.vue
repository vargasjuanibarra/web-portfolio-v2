<template>
  <div
    class="justify-between items-center md:p-8 md:flex w-full text-white mt-4 mb-12 my-auto md:min-h-[90vh]"
    id="main"
  >
    <div class="text-center pt-8 pb-4 flex flex-col gap-5 md:text-start px-4">
      <h1 class="text-4xl font-semibold text-wrap md:text-5xl lg:text-6xl">
        Hi I'm <span class="text-emerald-400">Juan </span> Vargas Fullstack
        <span class="text-emerald-400">Developer</span>
      </h1>
      <p>
        My Current Stack includes Typescript, Angular,
        <span class="text-emerald-400">Vue</span>, Svelte, Ionic, Tailwind,
        Node.js + Express, MongoDB, Prisma and Postgresql.
      </p>
      <div class="flex flex-col items-center pt-4">
        <a
          href="#contact"
          class="blueShadow mx-auto lg:mr-auto text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer"
        >
          <div
            class="absolute top-0 right-full w-full h-full bg-emerald-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
          />
          <h4 class="relative z-9">Get in touch &rarr;</h4>
        </a>
      </div>
    </div>
    <div class="p-2 mx-auto">
      <div class="relative shadow-lg grid place-items-center">
        <img
          src="../assets/profile.png"
          alt=""
          class="object-cover z-[2] min-h-[30vh] sm:max-w-[50vw] max-h-[30vh] md:max-h-[70vh] md:max-w-[40vw] lg:max-h-[50vh] lg:max-w-[40vw]"
        />
      </div>
    </div>
  </div>
</template>
<script>
particlesJS.load("particles-js", "/particles.json", function () {
  console.log("callback - particles.js config loaded");
});
</script>
<style lang=""></style>
