<template>
  <!-- Doctor card -->
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
          <i class="fab fa-facebook-square"></i>
        </a>
        <a href="#">
          <i class="fab fa-twitter-square"></i>
        </a>
        <a href="#">
          <i class="fab fa-instagram-square"></i>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "DoctorCard",
  props: ["doctor"],
};
</script>

<style lang="scss" scoped>
//// Import variables
@import "../scss/General/_vars.scss";
//// Import style card doctor
@import "../scss/Main/CardDoctorStyle.scss";
</style>