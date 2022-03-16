<template>
  <section-title
    style="margin-top: 30px"
    classHRef="fas fa-language"
    content="Languages"
  ></section-title>

  <skills-item skillName="Persian" progressValue="100"></skills-item>
  <skills-item skillName="English" progressValue="60"></skills-item>
  <skills-item skillName="Spanish" progressValue="5">
    <p>In progress</p>
  </skills-item>
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
p {
  display: block;
  font: 400 12px Roboto;
  text-align: right;
    color: var(--textColor);
}
</style>
