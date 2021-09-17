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

////Utility
.m-20 {
  margin-left: 20px;
}
.text-white {
  color: $white;
}

//// Appointments section style
#appointments {
  height: 86vh;
  background-image: url("../assets/images/make-an-appointment.jpg");
  background-position: center;
  background-size: cover;
  #form {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    margin: 0 auto;
    width: 500px;
    input {
      flex-basis: 200px;
      margin: 5px 2px;
      padding: 8px 6px;
      padding-right: 97px;
    }
    textarea,
    button {
      flex-basis: 495px;
    }
  }
}

//* Input type date
.container-date {
  border: 1px solid $primary-color;
  height: 30px;
  width: 245px;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  margin-left: 2px;
  #date {
    border: none;
    width: 100px;
  }
  .fa-calendar-alt {
    color: $grey;
    font-size: 10px;
    padding-left: 10px;
  }
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

//* Button form style
button {
  padding: 10px 0;
  margin: 10px 0;
  font-size: 12px;
  font-weight: lighter;
}
</style>