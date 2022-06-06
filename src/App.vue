<script setup>
import HeaderComp from "@/components/template/HeaderComp.vue";
import FooterComp from "@/components/template/FooterComp.vue";
</script>

<template>
  <HeaderComp />
  <main>
    <RouterView />
  </main>
  <FooterComp />
</template>

<style>
@import "@/assets/base.css";

body {
  background-color: rgba(218, 212, 212, 0.534);
}

#app {
  max-width: 1280px;
  margin: 0 auto;
  height: 100vh;
  /* padding: 2rem; */

  font-weight: normal;
}

footer {
  height: 10%;
  background-color: rgba(113, 182, 23, 0.473);
  color: white;
  font-size: 1.3rem;
  display: flex;
  align-items: center;
  padding-left: 15px;
}

.router-link-active {
  color: rgb(57, 192, 163);
}
</style>
