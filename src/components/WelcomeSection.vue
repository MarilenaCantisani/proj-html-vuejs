<template>
  <!-- Welcome section  -->
  <section id="welcome-section" class="container-small text-center">
    <!-- Title  -->
    <h3>Welcome to Avada Health</h3>
    <!-- Description -->
    <p class="description-section">
      Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium
      doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo
    </p>
    <!-- Info -->
    <Card :cards="welcomeInfo" id="card-welcome" />
  </section>
</template>

<script>
import Card from "@/components/Card.vue";
export default {
  name: "WelcomeSection",
  components: {
    Card,
  },
  data() {
    return {
      welcomeInfo: [
        {
          icon: require("@/assets/images/icon-1.png"),
          url: "#",
          title: "same day appointments",
          text: "Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium",
        },
        {
          icon: require("@/assets/images/icon-2.png"),
          url: "#",
          title: "world class facilities",
          text: "Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium",
        },
        {
          icon: require("@/assets/images/icon-3.png"),
          url: "#",
          title: "expert doctors",
          text: "Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium",
        },
        {
          icon: require("@/assets/images/icon-4.png"),
          url: "#",
          title: "complementary therapies",
          text: "Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
//// Import variables
@import "../scss/General/_vars.scss";
//// Import welcome section style
@import "../scss/Main/WelcomeStyle.scss";
</style>