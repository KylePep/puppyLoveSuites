<script setup>
const hours = ["Sunday|Closed", "Monday|8AM-6PM", "Tuesday|8AM-6PM", "Wednesday|8AM-6PM", "Thursday|8AM-6PM", "Friday|8AM-6PM", "Saturday|9AM-12PM",]

</script>

<template>
  <article>
    <h1>
      Contact Us!
    </h1>
    <ul>
      <li><span class="mdi mdi-home-variant fw-semibold"> Address:</span> 10330 Lake Shore Dr, Nampa, ID 83686
      </li>
      <li>
        <div class="accordion" id="accordionExample">
          <div class="accordion-item border border-0">
            <h2 class="accordion-header">
              <button class="accordion-button p-0 collapsed flex items-start pe-2" type="button"
                data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="false"
                aria-controls="collapseOne">
                <span class="mdi mdi-clock fw-semibold me-1"> Hours: </span>{{ ' ' + hours[new
                  Date().getDay()].split('|')[0]
                }}
                {{
                  hours[new Date().getDay()].split('|')[1] }}
              </button>
            </h2>
            <div id="collapseOne" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
              <div class="accordion-body">
                <ul>
                  <li v-for="hour in hours" :key="hour"> {{ ' ' + hour.split('|')[0]
                    }}
                    {{
                  hour.split('|')[1] }}</li>
                </ul>
              </div>
            </div>
          </div>
        </div>
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