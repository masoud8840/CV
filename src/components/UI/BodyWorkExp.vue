<template>
  <section class="v-body-work-exp">
    <body-title iconLink="fas fa-code" titleTxt="Work Experience"></body-title>
    <body-item
      job-title="Front End Developer / Freelancer"
      job-date="Jan 2021 - "
      :isCurrent="true"
      >I'm using my skills to do some practices as entertainment for myself and
      foreign project for having income.
    </body-item>
    <body-item
      job-title="Game Developer / brokenchair.blogfa.com"
      job-date="Jun 2018 - Sep 2018 "
      >Simple game development process i participated in it as a unity and c#
      developer.</body-item
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
.v-body-work-exp {
  padding: 10px 10px 0 10px;
  background-color: #fafafa;
}
</style>
