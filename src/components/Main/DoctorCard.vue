<template>
  <!-- DOCTOR CARD -->
  <div class="doctor-card clickable">
    <!-- Image  -->
    <img :src="doctor.profile" :alt="doctor.name" />
    <!-- Description  -->
    <div class="card-description">
      <h4 class="uppercase">{{ doctor.name }}</h4>
      <h5>{{ doctor.specialization }}</h5>
      <p>
        At vero eos et accusamus et iusto odio dignissimos ducisum qui
        blanditiis praesentium voluptatum deleniti atque
      </p>
      <!-- Social icon link -->
      <div class="social-icon">
        <a href="#">
          <i
            v-for="(social, index) in socialIcon"
            :key="index"
            class="fab"
            :class="social"
          >
          </i>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "DoctorCard",
  props: ["doctor", "socialIcon"],
};
</script>

<style lang="scss" scoped>
//// Import variables
@import "@/scss/General/_vars.scss";
//// Import style card doctor
@import "@/scss/Main/CardDoctorStyle.scss";
</style>