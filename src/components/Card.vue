<template>
  <div class="card" :id="id">
    <ul class="card-info">
      <!-- V-for to cycle in the data array "welcome-info" -->
      <li v-for="item in cards" :key="item.title">
        <a :href="item.url">
          <img :src="item.icon" :alt="item.title" />
          <h4 class="uppercase">{{ item.title }}</h4>
          <p>{{ item.text }}</p>
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: ["cards", "id"],
};
</script>

<style scoped lang="scss">
//// Import variables
@import "../scss/General/_vars.scss";
//// Cards import style
@import "../scss/Card/WelcomeCard.scss";
@import "../scss/Card/ServicesCard.scss";

//// General cards style
.card-info {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  flex-wrap: wrap;
  li {
    list-style-type: none;
    a {
      text-decoration: none;
    }
  }
}
</style>