<template>
  <section class="v-the-body">
    <work-exp></work-exp>
    <education-exp></education-exp>
  </section>
</template>

<script>
import WorkExp from "../UI/BodyWorkExp.vue";
import EducationExp from "../UI/EducationExp.vue";

export default {
  components: {
    WorkExp,
    EducationExp,
  },
};
</script>
<style lang="scss" scoped>
.v-the-body {
  margin-top: 10px;
}
</style>