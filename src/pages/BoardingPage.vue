<template>
  <div class="Hero row d-flex flex-column justify-content-center ">
    <h1 class="col-12 d-flex glassmorph text-white text-center flex-column justify-content-center flex-grow-1 mb-0">
      Boarding
    </h1>
  </div>
  <div class="row">
    <div class="col-12 px-0 text-center">
      <h2>Sweet Suites!</h2>
    </div>
  </div>

  <article class="row my-3 g-3">

    <div class="col-12">
      <h3 class="fw-bold">Dog Boarding</h3>
      Treat your furry friend to a luxurious getaway at Puppy Love Suites. Our spacious and comfortable suites provide
      the perfect home away from home for dogs of all shapes and sizes. // Heated and cooled suites.
    </div>

    <div>
      <h3>PRICES</h3>
      <table class="table table-hover ">
        <thead class="">
          <th scope="col">Description</th>
          <th scope="col">Rate</th>
        </thead>
        <tbody>

          <tr class="table-primary">
            <td scope="row">Suite 1st dog</td>
            <td>$40 per night</td>
          </tr>

          <tr class="">
            <td scope="row">Same suite additional dog(s)</td>
            <td>$33 per dog, per night</td>
          </tr>

          <tr class="table-primary">
            <td scope="row">Sunday and after hours pick up or drop off</td>
            <td>$50</td>
          </tr>

          <tr class="">
            <td scope="row">Medication administration</td>
            <td>$3 per day</td>
          </tr>

          <tr class="table-primary">
            <td scope="row">Food provided by Puppy Love Suites</td>
            <td>$5 per day</td>
          </tr>

        </tbody>
      </table>
    </div>

    <div class="col-12">
      <h4>FAQ</h4>
      <div class="row">

        <div class="col-12">
          <h5>What about the poop?</h5>
          <p>It gets cleaned up.</p>
        </div>

        <div class="col-12">
          <h5>What about cats?</h5>
          <p>What about cats.</p>
        </div>

        <div class="col-12">
          <h5>Do you have a good banana bread recipe?</h5>
          <p>I do but I won't tell you.</p>
        </div>

      </div>
    </div>

    <div class="col-12">
      <ContactUs />
    </div>

  </article>

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
article {
  margin: 2rem 0rem;

  >div {
    margin: 2rem 0rem;
  }
}

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