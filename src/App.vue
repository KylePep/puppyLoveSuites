<script setup>
import { AppState } from './AppState'
import Navbar from './components/Navbar.vue'


</script>

<template>
  <header>
    <Navbar />
  </header>
  <main class="container">
    <router-view />
  </main>
  <footer class="container-fluid d-flex bg-secondary text-light">
    <div class="row flex-grow-1 align-items-center">
      <p class="col-12 col-sm-6 text-center">
        Puppy Love Copyright Stuff
      </p>
      <div class="col-12 col-sm-6 text-center">
        <router-link :to="{ name: 'Contact' }" class="btn text-light lighten-30 selectable text-uppercase">
          Contact Us
        </router-link>
      </div>
    </div>
  </footer>
</template>

<style lang="scss">
@import "./assets/scss/main.scss";

:root {
  --main-height: calc(100vh - 32px - 64px);
}

footer {
  min-height: 128px;
}

h2 {
  background-color: var(--bs-primary);
  color: white;
  // text-shadow: 1px 1px 2px black;
  padding: 1rem 1rem 1rem 1rem;
  border-radius: 0px 0px 16px 16px;
}

.glassmorph {
  /* From https://css.glass */
  background: rgba(0, 0, 0, 0.35);
  // border-radius: 16px;
  // box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
  backdrop-filter: blur(1.25px);
  -webkit-backdrop-filter: blur(2px);
}
</style>
