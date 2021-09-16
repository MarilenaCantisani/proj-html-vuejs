<template>
  <main>
    <WelcomeSection />
    <Doctors />
    <Services />
    <Facilities />
  </main>
</template>

<script>
//// Import components main section
//* Import welcome section
import WelcomeSection from "@/components/WelcomeSection.vue";
//* Import doctors section
import Doctors from "@/components/Doctors.vue";
//* Import services section
import Services from "@/components/Services.vue";
//* Import facilities section
import Facilities from "@/components/Facilities.vue";

export default {
  name: "Main",
  components: {
    WelcomeSection,
    Doctors,
    Services,
    Facilities,
  },
};
</script>

<style>
</style>