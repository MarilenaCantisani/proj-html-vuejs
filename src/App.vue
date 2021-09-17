<template>
  <div id="app">
    <!-- Header -->
    <Header />
    <!-- Main -->
    <Main />
    <!-- Footer -->
    <Footer />
  </div>
</template>

<script>
//// Header component import
import Header from "@/components/Header/Header.vue";
//// Main component import
import Main from "@/components/Main/Main.vue";
//// Footer component import
import Footer from "@/components/Footer/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
};
</script>

<style lang="scss">
//// General style import
@import "./scss/General/generalStyle.scss";
</style>
