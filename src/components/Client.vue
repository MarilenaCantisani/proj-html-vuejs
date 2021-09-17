<template>
  <!-- Section client  -->
  <section id="client">
    <a href="#">
      <img
        v-for="(client, index) in clients"
        :key="index"
        :src="client.img"
        :alt="client.text"
        :id="client.text + index"
      />
    </a>
  </section>
</template>

<script>
export default {
  name: "Client",
  props: ["clients"],
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
    &:hover {
      transform: scale(1.1);
    }
  }
}
</style>