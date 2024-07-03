<template>
  <div class="bg-slate-900">
    <div class="max-w-[1200px] m-auto px-4">
      <Header />
      <Main></Main>
      <Projects id="projects"/>
      <AboutMe id="aboutme"/>
      <Experience  id="experience"/>
    </div>
    <Footer id="contact"/>
  </div>
</template>
<script setup>
import Header from './components/Header.component.vue';
import Main from './components/Main.component.vue';
import Projects from './components/Projects.component.vue';
import AboutMe from './components/About.component.vue';
import Experience from './components/Experience.component.vue';
import Footer from './components/Footer.component.vue';

</script>
<style lang="">
  
</style>