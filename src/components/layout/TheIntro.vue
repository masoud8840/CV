<template>
  <div class="container">
    <intro-spec></intro-spec>
    <div class="end-section-roll"></div>
    <intro-skills></intro-skills>
    <intro-languages></intro-languages>
  </div>
</template>
<script>
import IntroSpec from "../UI/IntroSpec.vue";
import IntroSkills from "../UI/IntroSkills.vue";
import IntroLanguages from "../UI/IntroLanguages.vue";

export default {
  components: {
    IntroSpec,
    IntroSkills,
    IntroLanguages,
  },
};
</script>
<style lang="scss" scoped>
.container {
  display: flex;
  flex-direction: column;
  box-shadow: 0 0 20px #eee;
  background-color: #fafafa;
  padding-bottom: 20px;

  .end-section-roll {
    width: 95%;
    height: 1px;
    background-color: #eee;
    margin-bottom: 20px;
    margin: 0 auto;
  }
}
</style>