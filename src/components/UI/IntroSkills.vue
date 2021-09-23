<template>
  <section>
    <section-title classHRef="far fa-keyboard" content="Skills"></section-title>
    <skills-item skillName="HTML (5), CSS (3)" progressValue="90"></skills-item>
    <skills-item skillName="SCSS" progressValue="90"></skills-item>
    <skills-item skillName="Bootstrap (5)" progressValue="90"></skills-item>
    <skills-item skillName="Javascript (ES6)" progressValue="65"></skills-item>
    <skills-item skillName="Vue.js (3)" progressValue="25"></skills-item>
  </section>
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