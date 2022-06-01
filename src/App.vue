<script></script>

<template>
  <header>
    <div class="menu-esquerdo">
      <span>Home</span>
      <span>|</span>
      <span>Times</span>
      <span>|</span>
      <span>Jogadores</span>
    </div>

    <div class="menu-direito">
      <span>Sair</span>
    </div>
  </header>
  <main>Bem-Vindo</main>
  <footer>Rodapé</footer>

  <RouterView />
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
  justify-content: space-between;
  padding-left: 15px;
}

main {
  height: 80%;
}

header span {
  padding: 0 20px;
}
</style>
