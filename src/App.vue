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

  <footer class="container-fluid d-flex bg-secondary text-light ">
    <div class="row flex-grow-1 align-items-center justify-content-center py-5">
      <div class="col-12 text-center fw-bold fs-4">
        <router-link :to="{ name: 'Home' }" class="text-light text-center selectable fw-bold fs-4">
          Puppy Love Suites
        </router-link>
      </div>

      <div class="col-6 d-flex justify-content-end px-0">
        <i class="mdi mdi-facebook fs-2 text-light py-1 px-2 selectable"></i>
        <i class="mdi mdi-instagram fs-2 text-light py-1 px-2 selectable"></i>
        <i class="mdi mdi-paw fs-2 text-light py-1 px-2 selectable"></i>
      </div>
      <div class="col-6 d-flex justify-content-start px-0">
        <p class="fs-6 fw-semibold text-light bg-primary rounded-4 px-2 py-2 mb-0 selectable ">(208) 353-5939</p>
      </div>
      <router-link :to="{ name: 'Contact' }" class="btn text-light lighten-30 selectable text-uppercase">
        10330 Lake Shore Dr, Nampa, ID 83686 | puppylovesuites@gmail.com
      </router-link>

      <div class="col-12">
        <p class=" text-center">
          Puppy Love Copyright Stuff
        </p>
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
  // min-height: 256px;
  margin-top: 32px;
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

/* Extra small devices (phones, 600px and down) */
@media only screen and (max-width: 600px) {
  article {
    padding: 0rem 1rem 0rem 1rem;
  }
}

/* Small devices (portrait tablets and large phones, 600px and up) */
@media only screen and (min-width: 600px) {
  article {
    padding: 0rem 3rem 0rem 3rem;
  }

  /* No changes needed */

}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {
  article {
    padding: 0rem 4rem 0rem 4rem;
  }

  /* No changes needed */

}

/* Large devices (laptops/desktops, 992px and up) */
@media only screen and (min-width: 992px) {
  article {
    padding: 0rem 6rem 0rem 6rem;
  }
}

/* Extra large devices (large laptops and desktops, 1200px and up) */
@media only screen and (min-width: 1200px) {
  article {
    padding: 0rem 12rem 0rem 12rem;
  }
}
</style>
