<template>
  <header class="bg-header">
    <!-- Header top -->
    <section id="header-bar" class="container">
      <!-- Logo  -->
      <a href="#">
        <img
          id="logo"
          src="@/assets/images/medical_logo_1x_light.png"
          alt="logo"
        />
      </a>
      <!-- Navigation bar  -->
      <nav>
        <ItemNav :nav="nav" />
      </nav>
    </section>
    <!-- Header bottom -->
    <section id="spotlight"></section>
  </header>
</template>

<script>
import ItemNav from "@/components/ItemNav.vue";
export default {
  name: "Header",
  components: {
    ItemNav,
  },
  data() {
    return {
      //// Navigation bar data array
      nav: [
        {
          id: "1",
          text: "home",
          url: "#",
          current: true,
        },
        {
          id: "2",
          text: "about",
          url: "#",
          current: false,
        },
        {
          id: "3",
          text: "departments",
          url: "#",
          current: false,
        },
        {
          id: "4",
          text: "articles",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
//// Import general style header
@import "../scss/Header/HeaderStyle.scss";
</style>