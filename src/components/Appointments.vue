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
        <input type="text" placeholder="Appointment Date" class="m-20" />
        <textarea
          name=""
          id=""
          cols="30"
          rows="10"
          placeholder="How can we help?*"
          required
        ></textarea>
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
#appointments {
  height: 80vh;
  background-image: url("../assets/images/make-an-appointment.jpg");
}
.text-white {
  color: $white;
}
#form {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  margin: 0 auto;
  width: 500px;
}
#form input {
  flex-basis: 200px;
  margin: 5px 2px;
  padding: 8px 10px;
  padding-right: 97px;
}
input,
textarea {
  background-color: transparent;
  border: 1px solid $primary-color;
  color: $white;
  font-size: 10px;
  padding: 8px 10px;
  font-weight: 200;
}

#form textarea,
button {
  flex-basis: 500px;
}
.m-20 {
  margin-left: 20px;
}
button {
  padding: 10px 0;
  margin: 10px 0;
  font-size: 12px;
  font-weight: lighter;
}
</style>