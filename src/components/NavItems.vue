<template>
  <div id="nav-bar">
    <ul>
      <!-- V-for to cycle in the data array of the nav-bar  -->
      <li v-for="item in nav" :key="item.id">
        <a :href="item.url" :class="{ active: item.current }" class="uppercase">
          {{ item.text }}
        </a>
      </li>
    </ul>
    <!-- Navigation bar button  -->
    <button class="uppercase clickable btn-light-blue" type="buttom">
      make appointment
    </button>
  </div>
</template>

<script>
export default {
  name: "NavItems",
  props: ["nav"],
};
</script>

<style lang="scss" scoped>
//// Import variables
@import "../scss/General/_vars.scss";
//// Import style navigation bar
@import "../scss/Header/NavStyle.scss";
</style>