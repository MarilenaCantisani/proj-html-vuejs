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
    <ul class="card-info">
      <!-- V-for to cycle in the data array "welcome-info" -->
      <li v-for="info in welcomeInfo" :key="info.title">
        <a :href="info.url">
          <img :src="info.icon" :alt="info.title" />
          <h4 class="uppercase">{{ info.title }}</h4>
          <p>{{ info.text }}</p>
        </a>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  name: "WelcomeSection",
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