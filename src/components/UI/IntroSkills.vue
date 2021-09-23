<template>
  <section>
    <section-title classHRef="far fa-keyboard" content="Skills"></section-title>
    <skills-item></skills-item>
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