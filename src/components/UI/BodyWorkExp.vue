<template>
  <section class="v-body-work-exp">
    <body-title iconLink="fas fa-code" titleTxt="Work Experience"></body-title>
    <body-item job-title="" :isCurrent="true"
      >Lorem ipsum dolor sit amet consectetur adipisicing elit. Laboriosam eius
      fugit explicabo dolores molestiae! Unde, itaque! Quasi obcaecati quas
      officiis?</body-item
    >
  </section>
</template>

<script>
import BodyTitle from "./UIComponents/BodyTitle.vue";
import BodyItem from "./UIComponents/BodyItem.vue";

export default {
  components: {
    BodyTitle,
    BodyItem,
  },
};
</script>

<style lang="scss" scoped>
</style>