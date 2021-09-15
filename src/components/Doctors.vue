<template>
  <!-- Doctors section -->
  <section id="doctors-section">
    <div class="container-small">
      <img src="../assets/images/icon-5.png" alt="logo-doctors" />
      <!-- Title -->
      <h3 class="uppercase">meet our doctors</h3>
      <!-- Description -->
      <p>
        Sed ut perspiciatis unde omnis iste natus error sit voluptatem
        accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab
        illo inventore veritatis et quasi architecto beatae
      </p>
      <article>
        <DoctorCard />
      </article>
    </div>
  </section>
</template>

<script>
import DoctorCard from "@/components/DoctorCard.vue";
export default {
  name: "Doctors",
  components: {
    DoctorCard,
  },
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
//// Import variables
@import "../scss/General/_vars.scss";
//// Import general style of doctors section
@import "../scss/Main/DoctorsStyle.scss";
</style>