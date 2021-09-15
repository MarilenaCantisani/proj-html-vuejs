<template>
  <section id="welcome-section">
    <h3>Welcome to Avada Health</h3>
    <p>
      Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium
      doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo
    </p>
    <ul>
      <li v-for="info in welcomeInfo" :key="info.title">
        <a :href="info.url">
          <img :src="info.icon" :alt="info.title" />
          <h4>{{ info.title }}</h4>
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

<style>
</style>