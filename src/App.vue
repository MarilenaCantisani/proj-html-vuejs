<template>
  <div id="app">
    <!-- Header -->
    <Header />
    <!-- Main -->
    <main>
      <WelcomeSection />
    </main>
  </div>
</template>

<script>
//// Header component import
import Header from "@/components/Header.vue";
import WelcomeSection from "@/components/WelcomeSection.vue";
export default {
  name: "App",
  components: {
    Header,
    WelcomeSection,
  },
};
</script>

<style lang="scss">
//// General style import
@import "./scss/General/generalStyle.scss";
</style>
