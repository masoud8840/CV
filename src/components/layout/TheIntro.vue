<template>
  <div class="container">
    <intro-spec></intro-spec>
  </div>
</template>
<script>
import IntroSpec from "../UI/IntroSpec.vue";

export default {
  components: {
    IntroSpec,
  },
};
</script>
<style lang="scss" scoped>
.container {
  display: flex;
  flex-direction: column;
}
</style>