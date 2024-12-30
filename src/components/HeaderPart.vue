<template>
    <section id="header">
        <header>
            <h1>キョウさんのポートフォリオ</h1>
            <nav>
                <ul>
                    <li><a href="#home">ホーム</a></li>
                    <li><a href="#about">自己紹介</a></li>
                    <li><a href="#contact">コンタクト</a></li>
                </ul>
            </nav>
        </header>
    </section>
</template>

<script>
    export default {
        name: "HeaderPart",
    };
</script>

<style>
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

</style>