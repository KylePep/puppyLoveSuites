<script setup>
import ContactUs from "../components/ContactUs.vue";


</script>

<template>
  <div class="Hero row d-flex flex-column justify-content-center ">
    <h1 class="col-12 d-flex glassmorph text-white text-center flex-column justify-content-center flex-grow-1 mb-0">
      About Us
    </h1>
  </div>

  <div class="row">
    <div class="col-12 px-0">
      <h2>his is the about us, it's all about us the onwers and operators of Puppy Love Suites.</h2>
    </div>
  </div>

  <div class="row">

    <div class="col-6">
      <h3>This is why you should trust me</h3>
      <ul>
        <li>Reason 1 </li>
        <li>Reason 2</li>
        <li>Reason 3</li>
      </ul>
    </div>

    <div class="col-6">
      <h3>This is why our services are better because of me</h3>
      <ul>
        <li>Reason 1 </li>
        <li>Reason 2</li>
        <li>Reason 3</li>
      </ul>
    </div>
  </div>

  <div class="row">
    <div class="col-12">
      <h4>This is why I do what I do.</h4>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugit nobis ipsa et in omnis laborum, fugiat a
        doloremque vero cupiditate. Eligendi, reiciendis. Consequuntur dicta minus neque veniam, vero numquam aperiam?
      </p>
    </div>
  </div>

  <ContactUs />
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