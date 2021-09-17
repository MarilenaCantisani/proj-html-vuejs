<template>
  <header class="bg-header">
    <!-- HEADER TOP -->
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
        <NavItems :nav="nav" />
      </nav>
    </section>
    <!-- HEADER BOTTOM -->
    <section id="spotlight" class="container-small">
      <div class="text-spotlight">
        <h2>
          <span>Caring </span>
          <span class="text-primary-color">For Life</span>
        </h2>
        <p>
          Kind words can be short and easy to speak, but their echoes are truly
          endless. Adava Health focuses on you as if it was our own family.
        </p>
        <button class="btn-spotlight uppercase btn-primary-color clickable">
          learn more
        </button>
      </div>
    </section>
  </header>
</template>

<script>
//// Nav component import
import NavItems from "@/components/Header/NavItems.vue";

export default {
  name: "Header",
  components: {
    NavItems,
  },
  data() {
    return {
      //* Navigation bar data array
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
//// Import variables
@import "@/scss/General/_vars.scss";
//// Import general style header
@import "@/scss/Header/HeaderStyle.scss";
//// Import spotlight style
@import "@/scss/Header/SpotlightStyle.scss";
</style>