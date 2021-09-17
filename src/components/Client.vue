<template>
  <!-- Section client  -->
  <section id="client">
    <img
      v-for="(client, index) in clients"
      :key="index"
      :src="client.img"
      :alt="client.text"
      :id="client.text + index"
    />
  </section>
</template>

<script>
export default {
  name: "Client",
  data() {
    return {
      clients: [
        {
          img: require("@/assets/images/client-logos-3.png"),
          text: "TurboPower",
        },
        {
          img: require("@/assets/images/client-logos-1.png"),
          text: "Healthy",
        },
        {
          img: require("@/assets/images/client-logos-4.png"),
          text: "Color People",
        },
        {
          img: require("@/assets/images/client-logos-2.png"),
          text: "Health",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
#client {
  height: 30vh;
  background-image: url("../assets/images/rgb-gradient-bar-for-logo-carrasel.jpg");
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0 auto;
  img {
    height: 160px;
  }
}
</style>