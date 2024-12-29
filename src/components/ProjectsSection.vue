<template>
    <section id="projects">
      <h2>プロジェクト</h2>
      <div v-for="project in projects" :key="project.id" class="project">
        <h3>{{ project.name }}</h3>
        <p>{{ project.description }}</p>
        <a :href="project.link" target="_blank">プロジェクトを見る</a>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: "ProjectsSection",
    data() {
      return {
        projects: [
          { id: 1, name: "プロジェクト1", description: "シンプルなプロジェクト例です。", link: "#" },
          { id: 2, name: "プロジェクト2", description: "もう1つのプロジェクト例です。", link: "#" },
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  .project {
    background: #fff;
    margin: 1rem 0;
    padding: 1rem;
    border-radius: 5px;
    box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
  }
  </style>