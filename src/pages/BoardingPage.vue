<template>
  <div class="Hero row d-flex flex-column justify-content-center ">
    <h1 class="col-12 d-flex glassmorph text-white text-center flex-column justify-content-center flex-grow-1 mb-0">
      Boarding
    </h1>
  </div>
  <div class="row">
    <div class="col-12 px-0 text-center">
      <h2>Remember that when you board with Puppy Love Suites you're boarding with the best!</h2>
    </div>
  </div>

  <div class="row my-3 g-3">

    <div class="col-12">
      <p class="fw-bold">Dog Boarding</p>
      Treat your furry friend to a luxurious getaway at Puppy Love Suites. Our spacious and comfortable suites provide
      the perfect home away from home for dogs of all shapes and sizes. With round-the-clock care and personalized
      attention from our dedicated staff, you can relax knowing that your pup is in good hands.
    </div>

    <div class="col-12 d-flex justify-content-center">
      <i class="separationMargin border-bottom border-2 border-primary w-75 align-items-center"> </i>
    </div>

    <div class="col-12">
      <p class="fw-bold">Daycare</p>
      Keep your dog entertained and socialized with our daycare services. Our supervised playgroups offer the perfect
      opportunity for dogs to romp, run, and make new friends in a safe and secure environment. Whether your pup loves
      chasing balls, playing tug-of-war, or just lounging in the sun, we'll make sure they have a tail-wagging good
      time.
    </div>

    <div class="col-12 d-flex justify-content-center">
      <i class="separationMargin border-bottom border-2 border-primary w-75 align-items-center"> </i>
    </div>

    <!-- <div class="col-12">
      <p class="fw-bold">Grooming</p>
      Treat your pup to a day of relaxation and rejuvenation with our professional grooming services. From baths and
      brush-outs to nail trims and ear cleanings, our experienced groomers will pamper your dog from head to tail,
      leaving them looking and feeling their best.
    </div>

    <div class="col-12">
      <p class="fw-bold">Training</p>
      Unlock your dog's full potential with our training programs. Whether you're dealing with behavioral issues,
      working on obedience commands, or simply want to strengthen the bond between you and your pup, our certified
      trainers are here to help. With positive reinforcement techniques and personalized attention, we'll set you and
      your dog up for success.
    </div> -->

    <div class="col-12">
      <p class="fw-bold">Specialized Care</p>
      We understand that every dog is unique, which is why we offer specialized care options to meet their individual
      needs. From medication administration to special dietary requirements, our team is equipped to handle any special
      requests to ensure your dog's health and happiness.
    </div>

    <div class="col-12 d-flex justify-content-center">
      <i class="separationMargin border-bottom border-2 border-primary w-75 align-items-center"> </i>
    </div>

    <div class="col-12">
      At Puppy Love Suites, we're dedicated to providing exceptional care and personalized attention to every dog who
      walks through our doors. Contact us today to learn more about our services and schedule your pup's next visit. Let
      us be your partner in your pet's well-being and happiness!
    </div>

    <div class="col-12">
      <ContactUs />
    </div>

  </div>

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

.separationMargin {
  margin: 1.5rem 0 1.5rem 0;
}
</style>