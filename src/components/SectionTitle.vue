<template>
  <div class="section-title">
    <!-- Icon section -->
    <img v-if="iconSection" :src="iconSection" :alt="title" />
    <!-- Title section-->
    <h3 class="uppercase">{{ title }}</h3>
    <!-- Description section-->
    <p v-if="!iconSection">
      Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium
      doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo
    </p>
    <p v-else>
      Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium
      doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo
      inventore veritatis et quasi architecto beatae
    </p>
  </div>
</template>

<script>
export default {
  name: "SectionTitle",
  props: ["title", "iconSection"],
};
</script>

<style lang="scss" scoped>
//// Import variables
@import "../scss/General/_vars.scss";
//// General style of of title section
@import "../scss/Main/TitleSectionStyle.scss";
</style>