<template>
  <section id="facilities">
    <div class="bg-section">
      <div class="container-small">
        <img src="../assets/images/icon-7.png" alt="facilities" />
        <!-- Title -->
        <h3 class="uppercase">tour our facilities</h3>
        <!-- Description -->
        <p>
          Sed ut perspiciatis unde omnis iste natus error sit voluptatem
          accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae
          ab illo inventore veritatis et quasi architecto beatae
        </p>
        <img
          id="play"
          class="clickable"
          src="@/assets/images/play-icon.png"
          alt="play"
        />
      </div>
    </div>

    <CardFacilities :cardInfo="facilitiesInfo" />
  </section>
</template>

<script>
import CardFacilities from "@/components/CardFacilities.vue";
export default {
  name: "Facilities",
  components: {
    CardFacilities,
  },
  data() {
    return {
      facilitiesInfo: [
        {
          title: "Emergency Care",
          icon: require("@/assets/images/wave-divider.png"),
          description:
            "Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque",
          textButton: "learn more",
          id: "emergency-care",
        },
        {
          title: "Expert diagnostics",
          icon: require("@/assets/images/wave-divider.png"),
          description:
            "Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque",
          textButton: "learn more",
          id: "expert-diagnostics",
        },
        {
          title: "Superb Rehabilitation",
          icon: require("@/assets/images/wave-divider.png"),
          description:
            "Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque",
          textButton: "learn more",
          id: "superb-rehabilitation",
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
#facilities {
  padding: 40px 0;
  color: $white;
  text-align: center;

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
#play {
  max-height: 40px;
  margin-top: 20px;
  &:hover {
    transform: scale(1.1);
  }
}
.bg-section {
  background-image: url("../assets/images/paralax-bg-tour-facilities.jpg");
  background-size: cover;
  background-position: center;
  height: 70vh;
}
</style>