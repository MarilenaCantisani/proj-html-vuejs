<template>
  <!-- Appointments section  -->
  <section id="appointments">
    <div class="container-small">
      <!-- Title -->
      <SectionTitle
        title="Make an Appointment"
        id="appointment"
        class="text-white"
      />
      <!-- Form -->
      <div id="form">
        <input type="text" placeholder="Name*" required />
        <input type="email" placeholder="Email*" required class="m-20" />
        <input type="text" placeholder="Phone Number" />
        <span class="container-date">
          <i class="fas fa-calendar-alt"></i>
          <input
            id="date"
            type="text"
            placeholder="Appointment Date"
            class="m-20"
          />
        </span>
        <textarea
          name=""
          id=""
          cols="30"
          rows="5"
          placeholder="How can we help?*"
          required
        ></textarea>
        <!-- Button form  -->
        <button class="btn-primary-color uppercase clickable">
          Make an appointment
        </button>
      </div>
    </div>
  </section>
</template>

<script>
//// Import component title section
import SectionTitle from "@/components/SectionTitle.vue";

export default {
  name: "Appointments",
  components: {
    SectionTitle,
  },
};
</script>

<style lang="scss" scoped>
//// Import variables
@import "../scss/General/_vars.scss";
//// Appointments section style
@import "../scss/Main/AppointmentsStyle.scss";
</style>