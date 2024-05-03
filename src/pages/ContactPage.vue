<script setup>
const days = ["Sun|Closed", "Mon|8AM-6PM", "Tue|8AM-6PM", "Wed|8AM-6PM", "Thu|8AM-6PM", "Fri|8AM-6PM", "Sat|9AM-12PM"]
const weekends = ["Sun|Closed", "Sat|9AM-12PM",]

</script>

<template>


  <article class="text-center">

    <div class="Hero d-flex flex-column justify-content-center text-light ">
      <h1>Contact Us!</h1>
    </div>

    <div class="d-flex flex-column">
      <h2 class="mdi mdi-clock fw-semibold"> Hours: </h2>
      <div class="d-flex flex-row justify-content-center">
        <div v-for="day in days" :key="day"
          :class="[day.split('|')[0] == 'Sun' || day.split('|')[0] == 'Sat' ? 'bg-gray' : 'bg-white', day.split('|')[0] == 'Sun' ? 'border-start-1 rounded-start' : 'border-start-0', day.split('|')[0] == 'Sat' ? 'rounded-end' : '']"
          class="d-flex flex-column border border-black text-center">
          <p class="bg-primary text-white px-2 py-1">{{ day.split('|')[0] }}</p>
          <div class="d-flex flex-column flex-sm-row">
            <p class="px-2 mb-0">{{ day.split('|')[1].split('-')[0] }}</p>
            <i v-if="day != 'Sun|Closed'">-</i>
            <p class="px-2">{{ day.split('|')[1].split('-')[1] }}</p>
          </div>
        </div>
      </div>
    </div>

    <div class="d-flex justify-content-center">
      <i class="separationMargin border-bottom border-2 border-primary w-75 my-5 align-items-center"> </i>
    </div>

    <div>
      <h2 class="mdi mdi-home-variant fw-semibold"> Address:
      </h2>
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2893.605939266819!2d-116.59967929999998!3d43.51055549999999!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x54ae49b3d5ccf939%3A0x7870a107ef3ae032!2sPuppy%20Love%20Suites!5e0!3m2!1sen!2sus!4v1714639389907!5m2!1sen!2sus"
        width="300" height="225" style="border:0;" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
      <p>10330 Lake Shore Dr, Nampa, ID 83686</p>
    </div>

    <div class="d-flex justify-content-center">
      <i class="border-bottom border-2 border-primary w-75 my-5 align-items-center"> </i>
    </div>


    <div>
      <h2 class="mdi mdi-phone fw-semibold"> Phone:
      </h2>
      <p>(208) 353-5939</p>
    </div>

    <div class="d-flex justify-content-center">
      <i class="border-bottom border-2 border-primary w-75 my-5 align-items-center"> </i>
    </div>


    <div>
      <h2 class="mdi mdi-email fw-semibold"> Email:
      </h2>
      <p>puppylovesuites@gmail.com</p>
    </div>
  </article>
</template>




<style lang="scss" scoped>
article>div {
  margin-bottom: 1rem;
}

.Hero {
  background-image: url(https://images.unsplash.com/photo-1586095088311-dc72701cc9cc?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D);
  background-position: bottom;
  background-size: cover;
  background-repeat: no-repeat;
  min-height: 10rem;
}

.separationMargin {}
</style>