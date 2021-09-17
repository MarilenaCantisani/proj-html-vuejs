<template>
  <!-- WELCOME SECTION -->
  <section id="welcome-section" class="container-small text-center">
    <!-- Title -->
    <SectionTitle title="Welcome to Adava Health" id="welcome" />
    <!-- Info -->
    <Card :cards="welcomeInfo" id="card-welcome" />
  </section>
</template>

<script>
//// Import component title section
import SectionTitle from "@/components/Main/SectionTitle.vue";
//// Import component card
import Card from "@/components/Main/Card.vue";

export default {
  name: "WelcomeSection",
  components: {
    SectionTitle,
    Card,
  },
  data() {
    return {
      //* Welcome info data array
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
@import "@/scss/General/_vars.scss";
//// Style welcome section
#welcome-section {
  margin-bottom: 30px;
}
//? Hover effects
.card-info li:hover a h4 {
  color: $primary-color;
}
.card-info li:hover a p {
  color: $dark-grey;
}
</style>