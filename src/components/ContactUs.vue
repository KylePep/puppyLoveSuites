<script setup>

</script>


<template>
  <!-- Button trigger modal -->
  <button type="button" class="btn btn-primary text-white" data-bs-toggle="modal" data-bs-target="#contactModal">
    ContactUs
  </button>

  <!-- Modal -->
  <div class="modal fade" id="contactModal" tabindex="-1" aria-labelledby="contactModalLabel" aria-hidden="true">
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h1 class="modal-title fw-bold fs-5" id="contactModalLabel">Contact Us</h1>
          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
        </div>
        <div class="modal-body">
          <ul>
            <li><span class="mdi mdi-home-variant fw-semibold"> Address:</span> 10330 Lake Shore Dr, Nampa, ID 83686
            </li>
            <li><span class="mdi mdi-clock fw-semibold"> Hours:</span> {{ new Date().toDateString() }}</li>
            <li><span class="mdi mdi-phone fw-semibold"> Phone:</span> (208) 353-5939</li>
            <li><span class="mdi mdi-email fw-semibold"> Email:</span> puppylovesuites@gmail.com</li>
          </ul>
          <p class="mx-5">
            Heres a blerb about contacting Puppy Love Suites.
          </p>
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
        </div>
      </div>
    </div>
  </div>

</template>


<style lang="scss" scoped>
ul {
  list-style-type: none;
}

ul>li {
  margin-top: 1rem;
}
</style>