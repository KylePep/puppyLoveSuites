<script>
import Hours from "../components/Hours.vue";


export default {
  data() {
    return {

    };

  },

};
</script>

<template>

  <div class="row Hero">
    <div class=" d-flex flex-column justify-content-center text-light text-center">
      <h1>Contact Us!</h1>
    </div>
  </div>


  <div class="row">
    <div class="col-12 px-0 text-center">
      <h2>We want to hear from you!</h2>
    </div>
  </div>

  <article class="row text-center my-3">
    <div class="col-12">
      We'd love to hear from you! Whether you have questions about our services, want to schedule a tour of our
      facilities, or just want to say hello, we're here to help. Get in touch with us using the contact information
      below:
      // Call to book etc
    </div>

    <div class="col-12 d-flex justify-content-center">
      <i class="separationMargin border-bottom border-2 border-primary w-100 align-items-center"> </i>
    </div>

    <div class="col-12">
      <div class="row">
        <h3 class="col-12 mdi mdi-phone fw-semibold"> Phone:
        </h3>
        <p class="col-12 col-md-5 mx-auto fs-5 fw-semibold btn text-white bg-primary px-2 py-1 rounded-4 selectable">
          (208) 353-5939</p>
      </div>
    </div>

    <div class="col-12 d-flex justify-content-center">
      <i class="separationMargin border-bottom border-2 border-primary w-100 align-items-center"> </i>
    </div>


    <div class="col-12">
      <div class="row">
        <h3 class="col-12 mdi mdi-email fw-semibold"> Email:
        </h3>
        <p class="col-12 col-md-5 mx-auto fs-5 fw-semibold btn text-white bg-primary px-3 py-1 rounded-4 selectable">
          puppylovesuites@gmail.com</p>
      </div>
    </div>

    <div class="col-12 d-flex justify-content-center">
      <i class="separationMargin border-bottom border-2 border-primary w-100 align-items-center"> </i>
    </div>

    <h3 class="col-12 mdi mdi-web fw-bold"> Connect with us:</h3>

    <div class="row mx-0 g-2">

      <div class="col-12 col-md-5 mx-auto fs-5 fw-semibold btn text-white bg-primary px-1 py-1 rounded-4 selectable">
        <i class="mdi mdi-instagram "></i> puppy_love_suites
      </div>

      <div class="col-12 col-md-5 mx-auto fs-5 fw-semibold btn text-white bg-primary px-1 py-1 rounded-4 selectable">
        <i class=" mdi mdi-facebook"></i> Puppy Love Suites
      </div>

    </div>


    <div class="col-12 d-flex justify-content-center">
      <i class="separationMargin border-bottom border-2 border-primary w-100 align-items-center"> </i>
    </div>

    <div class="col-12">
      <h3 class="mdi mdi-calendar-month fw-bold"> Schedule a Visit:</h3>
      <p class="mb-3">
        Ready to see Puppy Love Suites for yourself? We'd love to give you a tour of our facilities. Contact us today to
        schedule your visit and experience the Puppy Love Suites difference
        firsthand. <br> Thank you for considering Puppy Love Suites for your furry friend's care.
      </p>
      <i class="mdi mdi-paw fs-3 text-white bg-primary rounded-5 px-2 py-1"></i>
    </div>
    <!-- <p class="fs-5 fw-semibold btn text-white bg-primary px-3 py-1 rounded-4 selectable">//Call to schedule</p> -->

    <div class="col-12 d-flex justify-content-center">
      <i class="separationMargin border-bottom border-2 border-primary w-100 align-items-center"> </i>
    </div>

    <div class="col-12 d-flex flex-column">
      <h3 class="mdi mdi-clock fw-semibold"> Hours: </h3>

      <Hours />

    </div>

    <div class="col-12 d-flex justify-content-center">
      <i class="separationMargin border-bottom border-2 border-primary w-100 align-items-center"> </i>
    </div>

    <div class="col-12">
      <h3 class="mdi mdi-home-variant fw-semibold"> Address:
      </h3>
      <iframe class="border border-2 border-primary rounded"
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2893.605939266819!2d-116.59967929999998!3d43.51055549999999!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x54ae49b3d5ccf939%3A0x7870a107ef3ae032!2sPuppy%20Love%20Suites!5e0!3m2!1sen!2sus!4v1714639389907!5m2!1sen!2sus"
        width="100%" height="225" style="border:0;" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
      <p class="fw-semibold">10330 Lake Shore Dr, Nampa, ID 83686</p>
    </div>

  </article>
</template>




<style lang="scss" scoped>
article>div {
  margin-bottom: 1rem;
}

.Hero {
  background-image: url(https://images.unsplash.com/photo-1586095088311-dc72701cc9cc?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D);
  background-position: 95%;
  background-size: cover;
  background-repeat: no-repeat;
  min-height: 10rem;
}

.separationMargin {
  margin: 1.5rem 0 1.5rem 0;
}
</style>