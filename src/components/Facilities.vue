<template>
  <!-- Facilities section  -->
  <section id="facilities">
    <div class="bg-section">
      <div class="container-small">
        <!-- Title -->
        <SectionTitle
          title="tour our facilities"
          :iconSection="iconSection"
          class="text-white"
        />
      </div>
      <!-- Play icon  -->
      <div class="play-icon">
        <img class="clickable" src="@/assets/images/play-icon.png" alt="play" />
      </div>
    </div>
    <!-- Facilities sections  -->
    <FacilitiesSections :facilities="facilities" />
  </section>
</template>

<script>
//// Import component title section
import SectionTitle from "@/components/SectionTitle.vue";
//// Import component facilities section
import FacilitiesSections from "@/components/FacilitiesSections.vue";

export default {
  name: "Facilities",
  components: {
    SectionTitle,
    FacilitiesSections,
  },
  data() {
    return {
      iconSection: require("@/assets/images/icon-7.png"),
      facilities: [
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
//// General style of facilities section
@import "../scss/Main/FacilitiesStyle.scss";
</style>