<template>
  <section class="v-body-title">
    <i :class="iconLink"></i>
    <h1>{{ titleTxt }}</h1>
  </section>
</template>

<script>
export default {
  props: ["iconLink", "titleTxt"],
};
</script>
<style lang="scss" scoped>
.v-body-title {
  width: 100%;
  height: 7vh;
  display: flex;
  justify-content: flex-start;
  align-items: center;
  flex-direction: row;
  margin: 10px 0;
  i {
    font-size: 32px;
    padding: 10px 20px 10px 10px;
    color: #009688;
  }
  h1 {
    font: 400 30px Roboto;
    color: var(--textColor);
  }
}
</style>
