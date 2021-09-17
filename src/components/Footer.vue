<template>
  <footer>
    <Client />
    <InfoFooter />
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
};
</script>

<style>
</style>