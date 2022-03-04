<template>
  <section class="v-education-exp">
    <body-title
      iconLink="fas fa-graduation-cap"
      titleTxt="Education"
    ></body-title>
    <body-item
      job-title="Islamic Azad University / Islamshahr"
      job-date="Sep 2019 - "
      :isCurrent="true"
      >Bachelor Degree.</body-item
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
.v-education-exp {
  width: 100%;
  margin-top: 20px;
  background-color: #fafafa;
  padding: 10px 10px 0 10px;
}
</style>