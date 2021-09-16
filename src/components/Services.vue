<template>
  <section id="services">
    <div class="container-small">
      <img src="../assets/images/icon-6.png" alt="heart" />
      <!-- Title -->
      <h3 class="uppercase">our healt services</h3>
      <!-- Description -->
      <p>
        Sed ut perspiciatis unde omnis iste natus error sit voluptatem
        accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab
        illo inventore veritatis et quasi architecto beatae
      </p>
      <!-- Info -->
      <Card :cards="services" id="services" />
    </div>
  </section>
</template>

<script>
import Card from "@/components/Card.vue";

export default {
  name: "Services",
  components: {
    Card,
  },
  data() {
    return {
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
//// General style of doctors section
#services {
  padding: 40px 0;
  background-color: $white;
  text-align: center;
  color: $dark-grey;
  img {
    height: 60px;
  }
  h3 {
    font-size: 26px;
    font-weight: lighter;
    margin: 15px 0;
    //* Pseudoelement to create a separator
    &::after {
      content: "";
      width: 200px;
      border: 0.5px solid $light-grey;
      display: block;
      margin: 0 auto;
      margin-top: 20px;
    }
  }
  p {
    margin: 0 auto;
    width: 500px;
    line-height: 30px;
    font-weight: lighter;
    font-size: 17px;
    text-align: center;
  }
}
///
</style>