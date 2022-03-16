<template>
  <section>
    <section-title classHRef="far fa-keyboard" content="Skills"></section-title>
    <h3>as a Front End Developer:</h3>
    <skills-item
      skillName="HTML (5), CSS (3)"
      :progressValue="90"
    ></skills-item>
    <skills-item skillName="SCSS" :progressValue="90"></skills-item>
    <skills-item skillName="Tailwindcss (3)" :progressValue="30">
      <p>In progress</p>
    </skills-item>
    <skills-item skillName="Bootstrap (5)" :progressValue="90"></skills-item>
    <skills-item skillName="Javascript (ES6)" :progressValue="85">
    </skills-item>
    <skills-item skillName="Vue.js (3)" :progressValue="90"></skills-item>

    <h3>as a Back End Developer:</h3>
    <skills-item
      skillName="Node.js (16.10), Express.js (4)"
      progressValue="10"
    ></skills-item>
    <h3>Generals:</h3>
    <skills-item skillName="Git, Github" :progressValue="60">
      <p>Upgrading</p>
    </skills-item>
    <h3>Soft Skills:</h3>
    <skills-item skillName="Problem Solving" :progressValue="95"></skills-item>
    <skills-item skillName="Communication" :progressValue="90"></skills-item>
    <skills-item skillName="Self Learning" :progressValue="90"></skills-item>
    <skills-item skillName="Collaboration" :progressValue="90"></skills-item>
    <skills-item skillName="Time Management" :progressValue="75"></skills-item>
    <skills-item skillName="Patience" :progressValue="60"></skills-item>
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
p {
  display: block;
  font: 400 12px Roboto;
  text-align: right;
  color: var(--textColor);
}
h3 {
  color: var(--textColor);
  margin: 30px 0 0 20px;
  font: 600 15px Roboto;

  &:nth-child(2) {
    margin-top: 10px;
  }
}
</style>
