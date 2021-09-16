<template>
  <!-- Welcome section  -->
  <section id="welcome-section" class="container-small text-center">
    <!-- Title -->
    <SectionTitle title="Welcome to Adava Health" id="welcome" />
    <!-- Info -->
    <Card :cards="welcomeInfo" id="card-welcome" />
  </section>
</template>

<script>
//// Import component title section
import SectionTitle from "@/components/SectionTitle.vue";
//// Import component card
import Card from "@/components/Card.vue";

export default {
  name: "WelcomeSection",
  components: {
    SectionTitle,
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