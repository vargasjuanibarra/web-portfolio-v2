<template lang="">
<footer
  id="footer"
  class="py-20 sm:py-32 bg-black flex flex-col gap-4 sm:gap-8 justify-center items-center text-white"
>
  <p class="px-4 py-2 bg-white text-slate-950 font-medium">
    Connect with me &darr;
  </p>
  <div class="flex flex-col gap-4 items-center justify-center">
    <div
      class="flex items-center gap-4 sm:gap-6 text-2xl sm:text-3xl md:text-4xl mx-auto"
    >
      <a
        class="cursor-pointer"
        href="https://www.linkedin.com/in/juan-ibarra-vargas/"
        target="_blank"
      >
      <font-awesome-icon :icon="['fab', 'linkedin']" class="text-white"/>
      </a>
      <a
        class="cursor-pointer"
        href="https://github.com/vargasjuanibarra"
        target="_blank"
      >
        <font-awesome-icon :icon="['fab', 'github']" class="text-white"/>
      </a>
    </div>
    <p class="mx-auto text-sm opacity-70">or</p>

    <p>
      <b class="pr-2">Email:</b>
      <a
        href="mailto:vargasjuanibarra@gmail.com"
        target="_blank"
        class="text-emerald-400"
        >vargasjuanibarra@gmail.com
      </a>
    </p>

    <p>
      <b class="pr-2">GitHub</b>
      <a
        href="https://github.com/vargasjuanibarra"
        target="_blank"
        class="text-emerald-400"
        >vargasjuanibarra<sup class=""
          ><span class="text-xs scale-75 pl-0.5"
            ><i
              class="fa-solid fa-arrow-up-right-from-square text-xs scale-[75%]"
            />
            </span
          ></sup
        ></a
      >
    </p>
    <p>
      <b class="pr-2">LinkedIn</b>
      <a
        href="https://www.linkedin.com/in/juan-ibarra-vargas/"
        target="_blank"
        class="text-emerald-400"
        >Juan Vargas<sup class=""
          ><span class="text-xs scale-75 pl-0.5"
            ><i
              class="fa-solid fa-arrow-up-right-from-square text-xs scale-[75%]"
            /></span
          ></sup
        ></a
      >
    </p>
  </div>
</footer>

</template>
<script>
export default {
    
}
</script>
<style lang="">
    
</style>
