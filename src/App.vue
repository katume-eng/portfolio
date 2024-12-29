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
      <section id="home">
        <h1>キョウさんのポートフォリオ</h1>
      </section>
      <section id="projects">
        <h2>プロジェクト</h2>
        <div v-for="project in projects" :key="project.id" class="project">
          <h3>{{ project.name }}</h3>
          <p>{{ project.description }}</p>
          <a :href="project.link" target="_blank">プロジェクトを見る</a>
        </div>
      </section>
      <section id="about">
        <h2>About Me</h2>
        <p>ここに自己紹介を書くことができます。</p>
      </section>
      <section id="contact">
        <h2>コンタクト</h2>
        <p>連絡先情報をここに記載します。</p>
      </section>
    </main>
    <footer>
      <p>&copy; 2024 キョウさん</p>
    </footer>
  </div>
</template>

<script>
export default {
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
.project {
  background: #fff;
  margin: 1rem 0;
  padding: 1rem;
  border-radius: 5px;
  box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
}
a {
  color: #007BFF;
  text-decoration: none;
}
a:hover {
  text-decoration: underline;
}
footer {
  text-align: center;
  padding: 1rem;
  background: #333;
  color: #fff;
}
</style>