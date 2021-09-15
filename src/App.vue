<template>
  <div id="app">
    <!-- Header -->
    <Header />
    <!-- Main -->
    <main>
      <WelcomeSection />
      <Doctors />
    </main>
  </div>
</template>

<script>
//// Header component import
import Header from "@/components/Header.vue";
//// Import components main section
//* Import welcome section
import WelcomeSection from "@/components/WelcomeSection.vue";
//* Import doctors section
import Doctors from "@/components/Doctors.vue";

export default {
  name: "App",
  components: {
    Header,
    WelcomeSection,
    Doctors,
  },
};
</script>

<style lang="scss">
//// General style import
@import "./scss/General/generalStyle.scss";
</style>
