<template>
  <ul class="card-facilities">
    <li v-for="info in cardInfo" :key="info.title" :id="info.id">
      <h5>{{ info.title }}</h5>
      <img :src="info.icon" :alt="info.title" />
      <p>{{ info.description }}</p>
      <button>
        <a href="#">{{ info.textButton }}</a>
      </button>
    </li>
  </ul>
</template>

<script>
export default {
  name: "CardFacilities",
  props: ["cardInfo"],
};
</script>

<style lang="scss" scoped>
.card-facilities {
  display: flex;
  width: 100%;
  justify-content: space-evenly;
  align-items: center;
}
#emergency-care {
  background-color: #3aafbf;
}
#expert-diagnostics {
  background-color: #3597c3;
}
#superb-rehabilitation {
  background-color: #327ec7;
}
</style>