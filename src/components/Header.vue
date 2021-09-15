<template>
  <header class="bg-header">
    <!-- Header top -->
    <section id="header-bar" class="container">
      <img src="@/assets/images/medical_logo_1x_light.png" alt="logo" />
      <nav id="nav-bar"></nav>
    </section>
    <!-- Header bottom -->
    <section id="spotlight"></section>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      itemNav: [
        {
          id: "1",
          text: "home",
        },
        {
          id: "2",
          text: "about",
        },
        {
          id: "3",
          text: "departments",
        },
        {
          id: "4",
          text: "articles",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.bg-header {
  background-image: url("../assets/images/header-image-homepage.jpg");
}
</style>