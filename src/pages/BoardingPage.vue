<template>
  <div class="Hero row d-flex flex-column justify-content-center ">
    <h1 class="col-12 d-flex glassmorph text-white text-center flex-column justify-content-center flex-grow-1 mb-0">
      Boarding
    </h1>
  </div>
  <div class="row">
    <div class="col-12 px-0">
      <h2>Remember that when you board with Puppy Love Suites your boarding with the best!</h2>
    </div>
  </div>
  <ContactUs />
</template>


<script>
import ContactUs from "../components/ContactUs.vue";

export default {
  setup() {
    return {}
  }
}
</script>


<style lang="scss" scoped>
.Hero {
  background-image: url(https://images.unsplash.com/photo-1518640165980-d3e0e2aa6c1e?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D);
  background-position: 0% 80%;
  background-repeat: no-repeat;
  background-size: cover;
  min-height: 10rem;
}
</style>