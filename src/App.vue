<template>
  <div id="app">
    <HeaderPart />
    <main>
      <HomeSection />
      <ProjectsSection />
      <AboutSection />
      <ContactSection />
    </main>
    <FooterPart />
  </div>
</template>

<script>
import HomeSection from './components/HomeSection.vue';
import ProjectsSection from './components/ProjectsSection.vue';
import AboutSection from './components/AboutSection.vue';
import ContactSection from './components/ContactSection.vue';
import FooterPart from './components/FooterPart.vue';
import HeaderPart from './components/HeaderPart.vue';

export default {
  components: {
    HomeSection,
    ProjectsSection,
    AboutSection,
    ContactSection,
    FooterPart,
    HeaderPart,
  },
};
</script>

<style>
body {
  font-family: 'Arial', sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f4f4f4;
  color: #333;
}
main {
  padding: 2rem;
}
</style>