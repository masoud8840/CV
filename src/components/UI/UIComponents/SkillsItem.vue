<template>
  <section>
    <p>{{ skillName }}</p>
    <progress :value="progressValue" max="100"></progress>
    <slot></slot>
  </section>
</template>


<script>
export default {
  props: ["progressValue", "skillName"],
};
</script>
<style lang="scss" scoped>
section {
  width: 100%;
  padding: 0 20px;
  margin-top: 15px;
  progress {
    appearance: none;
    -webkit-appearance: none;
    width: 100%;
    height: 20px;
    margin-top: 15px;

    &::-webkit-progress-bar {
      appearance: none;
      background-color: #f1f1f1;
      border-radius: 25px;
    }
    &::-webkit-progress-value {
      appearance: none;
      background-color: #009688;
      border-radius: 25px;
    }
  }
  p {
    display: block;
    font: 400 15px Roboto;
    color: #757575;
  }
}
</style>    