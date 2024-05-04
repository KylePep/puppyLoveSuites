<script setup>
import ContactUs from "../components/ContactUs.vue";


</script>

<template>
  <div class="about">
    <div class="Hero row d-flex flex-column justify-content-center ">
      <h1 class="col-12 d-flex glassmorph text-white text-center flex-column justify-content-center flex-grow-1 mb-0">
        Boarding
      </h1>
    </div>
    <div class="row">
      <div class="col-12">
        <h2>his is the about us, it's all about us the onwers and operators of Puppy Love Suites.</h2>
      </div>
    </div>
    <ContactUs />
  </div>
</template>

<style scoped lang="scss">
.Hero {
  background-image: url(https://images.unsplash.com/photo-1642513730712-2ccba1dbef1e?q=80&w=1887&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D);
  background-position: 0% 20%;
  background-repeat: no-repeat;
  background-size: cover;
  min-height: 10rem;
}
</style>