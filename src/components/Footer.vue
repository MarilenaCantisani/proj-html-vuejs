<template>
  <footer>
    <Client />
    <InfoFooter :departments="departments" />
    <section id="copyright">
      <div class="container copy-container">
        <i class="far fa-copyright"></i>
        <div class="text-copyright">
          Copyright - 2020 | Adava Theme by
          <span class="text-dark-grey">Theme Fusion</span>
          | All Rights Reserved | Powered by
          <span class="text-dark-grey">Wordpress</span>
        </div>
      </div>
    </section>
  </footer>
</template>

<script>
import Client from "@/components/Client.vue";
import InfoFooter from "@/components/InfoFooter.vue";

export default {
  name: "Footer",
  components: {
    Client,
    InfoFooter,
  },
  data() {
    return {
      departments: [
        "Cardiology",
        "Pediactrics",
        "Diabetes Care",
        "Ultrasound Echocardiogram",
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
//// Import variables
@import "../scss/General/_vars.scss";
//// Utility
.text-dark-grey {
  color: $dark-grey;
}
//// Style copyright section
#copyright {
  background-color: $bg-section;
  .copy-container {
    display: flex;
    align-items: center;
    font-weight: lighter;
    font-size: 10px;
    i,
    .text-copyright {
      padding: 10px 0;
      margin-right: 2px;
      color: $grey;
    }
    i {
      font-size: 6px;
    }
  }
}
</style>