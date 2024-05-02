<script setup>
import { AppState } from './AppState'
import Navbar from './components/Navbar.vue'


</script>

<template>
  <header>
    <Navbar />
  </header>
  <main>
    <router-view />
  </main>
  <footer class="bg-secondary text-light">
    Puppy Love Copyright Stuff
  </footer>
</template>

<style lang="scss">
@import "./assets/scss/main.scss";

:root {
  --main-height: calc(100vh - 32px - 64px);
}

main {
  margin-left: 2rem;
  margin-right: 2rem;
}


footer {
  display: grid;
  place-content: center;
  height: 32px;
}
</style>
