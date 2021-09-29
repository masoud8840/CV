<template>
  <section>
    <section-title classHRef="far fa-keyboard" content="Skills"></section-title>
    <h5>as a Front End Developer:</h5>
    <skills-item skillName="HTML (5), CSS (3)" progressValue="90"></skills-item>
    <skills-item skillName="SCSS" progressValue="90"></skills-item>
    <skills-item skillName="Bootstrap (5)" progressValue="90"></skills-item>
    <skills-item skillName="Javascript (ES6)" progressValue="65"></skills-item>
    <skills-item skillName="Vue.js (3)" progressValue="25"
      ><p>In progress</p></skills-item
    >

    <h5>as a Back End Developer:</h5>
    <skills-item skillName="Node.js (16.10), Express.js (4)" progressValue="20"
      ><p>In progress</p></skills-item
    >

    <h5>as a Desktop Developer:</h5>
    <skills-item
      skillName="C# .NET Framework (4.8)"
      progressValue="35"
    ></skills-item>
    <skills-item
      skillName="C# .NET Core (2.2)"
      progressValue="35"
    ></skills-item>
    <skills-item skillName="C++" progressValue="35"></skills-item>
    <skills-item skillName="Unity 3D" progressValue="60"></skills-item>

    <h5>Generals:</h5>
    <skills-item skillName="Git, Github" progressValue="60"></skills-item>
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
  color: #757575;
}
h5 {
  color: #757575;
  margin: 30px 0 0 20px !important;
}
</style>