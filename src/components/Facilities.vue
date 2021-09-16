<template>
  <section id="facilities">
    <div class="bg-section">
      <div class="container-small">
        <SectionTitle
          title="tour our facilities"
          :iconSection="iconSection"
          class="text-white"
        />
      </div>
      <div class="icon-play">
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
import SectionTitle from "@/components/SectionTitle.vue";

export default {
  name: "Facilities",
  components: {
    SectionTitle,
    CardFacilities,
  },
  data() {
    return {
      iconSection: require("@/assets/images/icon-7.png"),
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
.icon-play {
  width: 100%;
  display: flex;
  justify-content: center;
}
#play {
  max-height: 40px;
  margin: 0 auto;
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
.text-white {
  color: $white;
}
</style>