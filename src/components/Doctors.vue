<template>
  <!-- Doctors section -->
  <section id="doctors-section">
    <div class="container-small">
      <SectionTitle title="meet our doctors" :iconSection="iconSection" />
      <!-- Section cards doctors -->
      <article>
        <ul class="card-container">
          <li v-for="doctor in doctors" :key="doctor.name">
            <DoctorCard :doctor="doctor" />
          </li>
        </ul>
      </article>
    </div>
  </section>
</template>

<script>
import DoctorCard from "@/components/DoctorCard.vue";
import SectionTitle from "@/components/SectionTitle.vue";
export default {
  name: "Doctors",
  components: {
    DoctorCard,
    SectionTitle,
  },
  data() {
    return {
      iconSection: require("@/assets/images/icon-5.png"),
      doctors: [
        {
          name: "Jon Snow",
          specialization: "Anesthesiologist",
          profile: require("@/assets/images/doctor-1.jpg"),
        },
        {
          name: "Tony Stark",
          specialization: "Cardiologist",
          profile: require("@/assets/images/doctor-2.jpg"),
        },
        {
          name: "Anna Smith",
          specialization: "Nurse Practitioner",
          profile: require("@/assets/images/doctor-3.jpg"),
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
//// Import variables
@import "../scss/General/_vars.scss";
//// Import general style of doctors section
@import "../scss/Main/DoctorsStyle.scss";
</style>