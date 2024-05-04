<template>
  <div v-if="isSmallScreen" class="d-flex flex-column justify-content-center align-items-center">
    <div v-for="day in longDays" :key="day"
      :class="[day.split('|')[0] == 'Sunday' || day.split('|')[0] == 'Saturday' ? 'bg-light' : 'bg-white', day.split('|')[0] == 'Sunday' ? 'border-bottom-1 rounded-top-1' : 'border-top-0', day.split('|')[0] == 'Saturday' ? 'rounded-bottom-1' : '']"
      class="d-flex flex-column border border-2 border-secondary w-75 text-center">
      <p class="bg-primary text-white fw-bold px-2 py-2 mb-0">{{ day.split('|')[0] }}</p>

      <div class="d-flex flex-row justify-content-center py-2">

        <div class="px-2">{{
    day.split('|')[1].split('-')[0] }}</div>
        <i v-if="day != 'Sunday|Closed'">-</i>
        <div v-if="day != 'Sunday|Closed'" class="px-2">{{ day.split('|')[1].split('-')[1] }}</div>

      </div>

    </div>

  </div>

  <div v-else class="d-flex flex-column flex-grow-1 align-items-center">
    <div class="d-flex flex-row w-100">
      <div v-for="day in longDays" :key="day"
        :class="[day.split('|')[0] == 'Sunday' || day.split('|')[0] == 'Saturday' ? 'bg-light' : 'bg-white', day.split('|')[0] == 'Sunday' ? 'border-start-2 rounded-start' : 'border-start-0', day.split('|')[0] == 'Saturday' ? 'rounded-end' : '']"
        class="d-flex flex-column flex-grow-1 border border-2 border-secondary text-center">
        <div class="bg-primary text-white fw-bold px-2 py-2">{{ day.split('|')[0] }}</div>

        <div class="d-flex flex-column flex-grow-1 ">
          <div class="px-2 ">{{
    day.split('|')[1].split('-')[0] }}</div>
          <i v-if="day != 'Sunday|Closed'" class="fw-semibold">-</i>
          <div v-if="day != 'Sunday|Closed'" class="px-2">{{ day.split('|')[1].split('-')[1] }} </div>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  setup() {
    return {
      screenWidth: window.innerWidth,
      shortDays: ["Sun|Closed", "Mon|8AM-6PM", "Tue|8AM-6PM", "Wed|8AM-6PM", "Thu|8AM-6PM", "Fri|8AM-6PM", "Sat|9AM-12PM"],
      longDays: ["Sunday|Closed", "Monday|8AM-6PM", "Tuesday|8AM-6PM", "Wednesday|8AM-6PM", "Thursday|8AM-6PM", "Friday|8AM-6PM", "Saturday|9AM-12PM"]
    }
  },
  computed: {
    isSmallScreen() {
      return this.screenWidth < 768;
    }
  },
  mounted() {
    // Update screenWidth when the window is resized
    window.addEventListener('resize', this.updateScreenWidth);
  },
  methods: {
    updateScreenWidth() {
      this.screenWidth = window.innerWidth;
    }
  },
  beforeUnmount() {
    // Remove event listener to prevent memory leaks
    window.removeEventListener('resize', this.updateScreenWidth);
  }
}
</script>


<style lang="scss" scoped></style>