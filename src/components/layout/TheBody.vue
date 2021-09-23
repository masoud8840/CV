<template>
  <section class="v-the-body">
    <work-exp></work-exp>
  </section>
</template>

<script>
import WorkExp from "../UI/BodyWorkExp.vue";

export default {
  components: {
    WorkExp,
  },
};
</script>
<style lang="scss" scoped>
section.v-the-body {
  margin-top: 10px;
  padding: 10px;
  background-color: #fafafa;
}
</style>