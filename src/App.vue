<template>
  <div id="app">
    <!-- Header -->
    <Header />
    <!-- Main -->
    <Main />
  </div>
</template>

<script>
//// Header component import
import Header from "@/components/Header.vue";
import Main from "@/components/Main.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
  },
};
</script>

<style lang="scss">
//// General style import
@import "./scss/General/generalStyle.scss";
</style>
