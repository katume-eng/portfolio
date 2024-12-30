<template>
  <div id="app">
    <header>
      <nav>
        <ul>
          <li><a href="#home">ホーム</a></li>
          <li><a href="#projects">プロジェクト</a></li>
          <li><a href="#about">About Me</a></li>
          <li><a href="#contact">コンタクト</a></li>
        </ul>
      </nav>
    </header>
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

export default {
  components: {
    HomeSection,
    ProjectsSection,
    AboutSection,
    ContactSection,
    FooterPart,
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
header {
  background-color: #333;
  color: #fff;
  padding: 1rem;
}
nav ul {
  list-style: none;
  display: flex;
  justify-content: center;
  gap: 1rem;
  padding: 0;
  margin: 0;
}
nav ul li {
  display: inline;
}
nav ul li a {
  color: #fff;
  text-decoration: none;
  font-weight: bold;
}
nav ul li a:hover {
  text-decoration: underline;
}
main {
  padding: 2rem;
}
</style>