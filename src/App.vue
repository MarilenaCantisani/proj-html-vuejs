<template>
  <div id="app">
    <!-- Header -->
    <Header />
  </div>
</template>

<script>
//// Header component import
import Header from "@/components/Header.vue";
export default {
  name: "App",
  components: {
    Header,
  },
};
</script>

<style lang="scss">
//// General style import
@import "./scss/General/generalStyle.scss";
</style>
