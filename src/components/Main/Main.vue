<template>
  <main>
    <WelcomeSection />
    <Doctors />
    <Services />
    <Facilities />
    <Appointments />
  </main>
</template>

<script>
//// Import components main section
//* Import welcome section
import WelcomeSection from "@/components/Main/WelcomeSection.vue";
//* Import doctors section
import Doctors from "@/components/Main/Doctors.vue";
//* Import services section
import Services from "@/components/Main/Services.vue";
//* Import facilities section
import Facilities from "@/components/Main/Facilities.vue";
//* Import appointments section
import Appointments from "@/components/Main/Appointments.vue";

export default {
  name: "Main",
  components: {
    WelcomeSection,
    Doctors,
    Services,
    Facilities,
    Appointments,
  },
};
</script>
