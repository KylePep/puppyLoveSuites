<script setup>
import ContactUs from '../components/ContactUs.vue'
</script>

<template>
  <div class="flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <h1>Welcome to Puppy Love Suites</h1>
    <p>Drop your dogs off, they deserve a vacation from you too!</p>
    <ContactUs />
  </div>
</template>

<style scoped lang="scss">
.home {
  display: grid;
  height: 80vh;
  place-content: center;
  text-align: center;
  user-select: none;

  .home-card {
    width: clamp(500px, 50vw, 100%);

    >img {
      height: 200px;
      max-width: 200px;
      width: 100%;
      object-fit: contain;
      object-position: center;
    }
  }
}
</style>
