<template>
  <div class="container">
    <intro-spec></intro-spec>
    <div class="end-section-roll"></div>
    <intro-skills></intro-skills>
  </div>
</template>
<script>
import IntroSpec from "../UI/IntroSpec.vue";
import IntroSkills from "../UI/IntroSkills.vue";

export default {
  components: {
    IntroSpec,
    IntroSkills,
  },
};
</script>
<style lang="scss" scoped>
.container {
  display: flex;
  flex-direction: column;
  .end-section-roll {
    width: 95%;
    height: 1px;
    background-color: #eee;
    margin-bottom: 20px;
  }
}
</style>