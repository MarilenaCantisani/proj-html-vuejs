<template>
  <!-- FACILITY SECTION -->
  <ul class="facility">
    <li v-for="facility in facilities" :key="facility.title" :id="facility.id">
      <h5>{{ facility.title }}</h5>
      <img :src="facility.icon" :alt="facility.title" />
      <p>{{ facility.description }}</p>
      <button class="clickable">
        <a class="uppercase" href="#">
          {{ facility.textButton }}
        </a>
      </button>
    </li>
  </ul>
</template>

<script>
export default {
  name: "FacilitiesSections",
  props: ["facilities"],
};
</script>

<style lang="scss" scoped>
//// Import variables
@import "@/scss/General/_vars.scss";
//// Import general style of facility
@import "@/scss/Main/FacilityStyle.scss";
</style>