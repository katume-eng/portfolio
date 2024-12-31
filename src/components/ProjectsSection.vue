<template>
  <section id="projects">
    <h2>プロジェクト</h2>  
    <div class="project-cards">
      <div v-for="project in projects" :key="project.id" class="card">
        <a :href="project.link" target="_blank">
        <img src="project.image" alt="project.name"/>
        <div class="card-content">
        <h3>{{ project.name }}</h3>
        <p>{{ project.description }}</p>
        </div>
        </a>
      </div>  
    </div>
  </section>
</template>
  
  <script>
  export default {
    name: "ProjectsSection",
    data() {
      return {
        projects: [
          { 
            id: 1,
            name: "プロジェクト1",
            description: "シンプルなプロジェクト例です。",
            link: "#",
            image: "##",
          },
          { 
            id: 2,
            name: "プロジェクト2",
            description: "もう1つのプロジェクト例です。",
            link: "#",
            image: "##",
          },
          { 
            id: 3,
            name: "プロジェクト3",
            description: "最後のプロジェクト例です。",
            link: "#",
            image: "##",
          },
          {
            id: 4,
            name: "プロジェクト4",
            description: "最後のプロジェクト例です。",
            link: "#",
            image: "##",
          },
          {
            id: 5,
            name: "プロジェクト5",
            description: "最後のプロジェクト例です。",
            link: "#",
            image: "##",
          },
          {
            id: 6,
            name: "プロジェクト6",
            description: "最後のプロジェクト例です。",
            link: "#",
            image: "##",
          },
          {
            id: 7,
            name: "プロジェクト7",
            description: "最後のプロジェクト例です。",
            link: "#",
            image: "##",
          },
          {
            id: 8,
            name: "プロジェクト8",
            description: "最後のプロジェクト例です。",
            link: "#",
            image: "##",
          },
          {
            id: 9,
            name: "プロジェクト9",
            description: "最後のプロジェクト例です。",
            link: "#",
            image: "##",
          },
          {
            id: 10,
            name: "プロジェクト10",
            description: "最後のプロジェクト例です。",
            link: "#",
            image: "##",
          },
          {
            id: 11,
            name: "プロジェクト11",
            description: "最後のプロジェクト例です。",
            link: "#",
            image: "##",
          },
          {
            id: 12,
            name: "プロジェクト12",
            description: "最後のプロジェクト例です。",
            link: "#",
            image: "##",
          },
          {
            id: 13,
            name: "プロジェクト13",
            description: "最後のプロジェクト例です。",
            link: "#",
            image: "##",
          },
          {
            id: 14,
            name: "プロジェクト14",
            description: "最後のプロジェクト例です。",
            link: "#",
            image: "##",
          },
          {
            id: 15,
            name: "プロジェクト15",
            description: "最後のプロジェクト例です。",
            link: "#",
            image: "##",
          },
          {
            id: 16,
            name: "プロジェクト16",
            description: "最後のプロジェクト例です。",
            link: "#",
            image: "##",
          },
          {
            id: 17,
            name: "プロジェクト17",
            description: "最後のプロジェクト例です。",
            link: "#",
            image: "##",
          },
          {
            id: 18,
            name: "プロジェクト18",
            description: "最後のプロジェクト例です。",
            link: "#",
            image: "##",
          },
          {
            id: 19,
            name: "プロジェクト19",
            description: "最後のプロジェクト例です。",
            link: "#",
            image: "##",
          },
          {
            id: 20,
            name: "プロジェクト20",
            description: "最後のプロジェクト例です。",
            link: "#",
            image: "##",
          },
        ],
      };
    },
  };
  </script>
  
<style>
  .project-cards {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  justify-content: center;
}

.card {
  padding: 16px;
  background: linear-gradient(135deg, #85bffa, #b0c1f5); /* グラデーション */
  border: 1px solid #c6c1c100;
  border-radius: 8px;
  width: 300px;
  overflow: hidden;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  transition: transform 0.2s ease-in-out;
}

.card:hover {
  transform: scale(1.05);
}

.card img {
  width: 100%;
  height: auto;
}

.card-content {
  padding: 16px;
}

.card-content h3 {
  margin: 0 0 8px;
}

.card-content p {
  color: #555;
  font-size: 0.9em;
}
</style>