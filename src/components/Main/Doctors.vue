<template>
  <!-- DOCTORS SECTION -->
  <section id="doctors-section">
    <div class="container-small">
      <SectionTitle title="meet our doctors" :iconSection="iconSection" />
      <!-- Section cards doctors -->
      <article>
        <ul class="card-container">
          <li v-for="doctor in doctors" :key="doctor.name">
            <DoctorCard :doctor="doctor" :socialIcon="socialIcon" />
          </li>
        </ul>
      </article>
    </div>
  </section>
</template>

<script>
//// Import component title section
import SectionTitle from "@/components/Main/SectionTitle.vue";
//// Import component card doctor
import DoctorCard from "@/components/Main/DoctorCard.vue";

export default {
  name: "Doctors",
  components: {
    DoctorCard,
    SectionTitle,
  },
  data() {
    return {
      iconSection: require("@/assets/images/icon-5.png"),
      //* Doctors data array
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
      //* Social data array
      socialIcon: [
        "fa-facebook-square",
        "fa-twitter-square",
        "fa-instagram-square",
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
//// Import variables
@import "@/scss/General/_vars.scss";

//// Style doctors section
#doctors-section {
  background-color: $bg-section;
}
//* Style card container
.card-container {
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  li {
    list-style-type: none;
  }
}
</style>