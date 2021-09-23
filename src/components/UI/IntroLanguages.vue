<template>
  <section-title
    style="margin-top: 30px"
    classHRef="fas fa-language"
    content="Languages"
  ></section-title>

  <skills-item skillName="Persian" progressValue="100"></skills-item>
  <skills-item skillName="English" progressValue="60"></skills-item>
  <skills-item skillName="Spanish" progressValue="5"></skills-item>
</template>

<script>
import SectionTitle from "./UIComponents/SectionTitle.vue";
import SkillsItem from "./UIComponents/SkillsItem.vue";

export default {
  components: {
    SectionTitle,
    SkillsItem,
  },
};
</script>
<style lang="scss" scoped>
</style>
