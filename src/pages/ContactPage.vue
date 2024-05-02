<script setup>
const hours = ["Sunday|Closed", "Monday|8AM-6PM", "Tuesday|8AM-6PM", "Wednesday|8AM-6PM", "Thursday|8AM-6PM", "Friday|8AM-6PM", "Saturday|9AM-12PM",]

</script>

<template>
  <article>
    <h1>
      Contact Us!
    </h1>
    <ul>

      <li class="d-flex flex-column">
        <h2 class="mdi mdi-clock fw-semibold"> Hours: </h2>
        <div class="d-flex flex-row justify-content-around">
          <div v-for="hour in hours" :key="hour"
            class="d-flex flex-grow-1 flex-column border borer-1 border-black text-center">
            <p class="bg-primary text-white px-2 py-1">{{ hour.split('|')[0] }}</p>
            <div class="px-2 py-1">{{ hour.split('|')[1] }}</div>
          </div>
        </div>
      </li>


      <li><span class="mdi mdi-home-variant fw-semibold"> Address:</span> 10330 Lake Shore Dr, Nampa, ID 83686
      </li>
      <li>
      </li>
      <li><span class="mdi mdi-phone fw-semibold"> Phone:</span> (208) 353-5939</li>
      <li><span class="mdi mdi-email fw-semibold"> Email:</span> puppylovesuites@gmail.com</li>
    </ul>
  </article>
</template>




<style lang="scss" scoped>
ul {
  list-style-type: none;
}

ul>li {
  margin-top: 1rem;
}
</style>