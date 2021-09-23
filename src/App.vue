<template>
  <div class="container">
    <the-intro></the-intro>
    <the-body></the-body>
  </div>
</template>

<script>
import TheIntro from "./components/layout/TheIntro.vue";
import TheBody from "./components/layout/TheBody.vue";

export default {
  components: {
    TheIntro,
    TheBody,
  },
  name: "App",
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@100;400;700&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Roboto, sans-serif;
}

.container {
  width: 100%;
  max-width: 1450px;
  height: fit-content;
  margin: 0 auto;
  padding: 10px;
  display: grid;
  grid-template-columns: 2fr 4fr;
  column-gap: 25px;
}
</style>
