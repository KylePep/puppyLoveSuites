<script setup>
import PhotoCarousel from '../components/PhotoCarousel.vue'
import ContactUs from '../components/ContactUs.vue'
</script>

<template>
  <div class="Hero row d-flex flex-column justify-content-center">
    <div class="col-12 d-flex glassmorph text-white text-center flex-column justify-content-center flex-grow-1">
      <h1 class="">Welcome to Puppy Love Suites</h1>

      <p class="">Drop your dogs off, they deserve a vacation from you too!</p>
    </div>
  </div>

  <div class="row">
    <div class="col-12 px-0">
      <h2 class="text-center">
        Top-quality pet boarding in Nampa!
      </h2>
    </div>
  </div>

  <article class="row g-2 my-3">

    <PhotoCarousel />

    <!-- <Notification /> -->


    <div class="col-12">
      At Puppy Love Suites, we understand that your furry friend is more than just a pet – they're a cherished member of
      your family. That's why we provide top-notch dog boarding services designed to pamper your pooch and give you
      peace of mind while you're away.
    </div>

    <div class="col-12">
      Our luxury suites offer a cozy retreat for your beloved companion, complete with heated floors in the chilly
      months and air conditioning in the summer, personalized attention, and plenty of playtime in our secure,
      supervised indoor and outdoor areas. Whether your pup prefers romping around with new friends or simply lounging
      in the sunshine, we cater to their every need and preference.
    </div>

    <div class="col-12">
      Safety is our top priority, which is why our facility is equipped with state-of-the-art security measures and
      staffed by trained professionals who are passionate about caring for dogs. You can rest assured knowing that your
      furry friend is in good hands during their stay with us.
    </div>

    <div class="col-12">
      Beyond exceptional care, we also strive to create a welcoming and inclusive environment for both dogs and their
      humans. We believe in building relationships with our clients based on trust, transparency, and genuine compassion
      for animals.
    </div>

    <div class="col-12">
      So whether you're heading out of town for a weekend getaway or a longer vacation, trust Puppy Love Suites to
      provide the love, attention, and care your dog deserves. Contact us today to schedule a tour of our facilities or
      reserve a spot for your furry friend's next stay. Let us be your dog's home away from home!
    </div>

    <div class="col-12">
      <ContactUs />
    </div>
  </article>
</template>

<style scoped lang="scss">
.Hero {
  background-image: url(https://images.unsplash.com/photo-1581888227599-779811939961?q=80&w=1074&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D);
  background-position: 0% 60%;
  background-repeat: no-repeat;
  background-size: cover;
  min-height: 10rem;
}

.dismiss:hover {
  cursor: pointer;
  color: var(--bs-secondary);
}
</style>
