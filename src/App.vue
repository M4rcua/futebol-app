<script></script>

<template>
  <header>
    <span class="texto-header">Home</span>
    <span class="separador">|</span>
    <span class="texto-header">Times</span>
    <span class="separador">|</span>
    <span class="texto-header">Jogadores</span>
  </header>
  <main>main</main>
  <footer>Rodapé</footer>
</template>

<style>
@import "@/assets/base.css";

body {
  background-color: gray;
}

#app {
  max-width: 1280px;
  margin: 0 auto;
  height: 100vh;
  /* padding: 2rem; */

  font-weight: normal;
}

header,
footer {
  height: 10%;
  background-color: rgb(57, 57, 128);
  color: white;
  font-size: 1.3rem;
  display: flex;
  align-items: center;
  padding-left: 15px;
}

main {
  height: 80%;
}

header span {
  padding: 0 20px;
}
</style>
