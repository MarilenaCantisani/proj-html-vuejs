<template>
  <footer>
    <Client />
    <InfoFooter :departments="departments" />
  </footer>
</template>

<script>
import Client from "@/components/Client.vue";
import InfoFooter from "@/components/InfoFooter.vue";

export default {
  name: "Footer",
  components: {
    Client,
    InfoFooter,
  },
  data() {
    return {
      departments: [
        "Cardiology",
        "Pediactrics",
        "Diabetes Care",
        "Ultrasound Echocardiogram",
      ],
    };
  },
};
</script>

<style>
</style>