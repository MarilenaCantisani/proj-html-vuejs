<template>
  <section id="services">
    <div class="container-small">
      <SectionTitle title="our health services" :iconSection="iconSection" />
      <!-- Info -->
      <Card :cards="services" id="services" />
    </div>
  </section>
</template>

<script>
import Card from "@/components/Card.vue";
import SectionTitle from "@/components/SectionTitle.vue";

export default {
  name: "Services",
  components: {
    SectionTitle,
    Card,
  },
  data() {
    return {
      iconSection: require("@/assets/images/icon-6.png"),
      services: [
        {
          icon: require("@/assets/images/icon-14.png"),
          url: "#",
          title: "rehabilitation center",
          text: "At vero eos et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos dolores et quas",
        },
        {
          icon: require("@/assets/images/icon-15.png"),
          url: "#",
          title: "dental implants",
          text: "At vero eos et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos dolores et quas",
        },
        {
          icon: require("@/assets/images/icon-16.png"),
          url: "#",
          title: "medicine research",
          text: "At vero eos et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos dolores et quas",
        },
        {
          icon: require("@/assets/images/icon-11.png"),
          url: "#",
          title: "blood bank",
          text: "At vero eos et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos dolores et quas",
        },
        {
          icon: require("@/assets/images/icon-12.png"),
          url: "#",
          title: "pharmaceutical advice",
          text: "At vero eos et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos dolores et quas",
        },
        {
          icon: require("@/assets/images/icon-13.png"),
          url: "#",
          title: "medical counseling",
          text: "At vero eos et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos dolores et quas",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
//// Import variables
@import "../scss/General/_vars.scss";
</style>