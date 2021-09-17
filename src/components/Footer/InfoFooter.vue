<template>
  <!-- INFO-FOOTER SECTION -->
  <section id="info-footer">
    <div class="adava-info container">
      <!-- Social  -->
      <div class="col social-info">
        <a href="#">
          <img src="@/assets/images/medical_logo_1x_dark.png" alt="adava" />
        </a>
        <p>
          Sed ut perspiciatis unde omnis iste natus error sit voluptatem
          accusantium dolemue launti totam aperiam, eaque ipsa quae abillo.
          Invente veriatis et quasi architecto beatae luptatem accusantium,
          remaperiamsiat. Voluptatem accusest etsium doloremque laudaien. Lorem
          ipsum sits dolores ets unser.
        </p>
        <span class="uppercase">learn more about us</span>
        <div class="social-icon">
          <a href="#">
            <i
              v-for="(social, index) in socialClass"
              :key="index"
              class="fab"
              :class="social"
            ></i>
          </a>
        </div>
      </div>
      <!-- Contact  -->
      <div class="col contact-info">
        <h6 class="uppercase">contact information</h6>
        <div>
          <i class="fas fa-map-marker-alt"></i>
          <address class="clickable">
            121king Street, London United Kingdom
          </address>
        </div>
        <div>
          <i class="fas fa-phone"></i>
          <span class="clickable">1.800.458.556</span>
        </div>
      </div>
      <!-- Departments -->
      <div class="col departments-info">
        <h6 class="uppercase">medical depaertments</h6>
        <ul>
          <li v-for="(department, index) in departments" :key="index">
            <i class="fas fa-chevron-circle-right"></i>
            <a href="#" class="clickable">
              {{ department }}
            </a>
          </li>
        </ul>
        <button class="uppercase clickable">View our departments</button>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "InfoFooter",
  props: ["departments"],
  data() {
    return {
      //* Social data array
      socialClass: [
        "fa-facebook-square",
        "fa-twitter-square",
        "fa-youtube-square",
        "fa-instagram-square",
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
//// Import variables
@import "@/scss/General/_vars.scss";
//// Import footer style
@import "@/scss/Footer/FooterStyle.scss";
</style>