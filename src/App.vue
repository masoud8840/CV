<template>
  <div class="container">
    <the-intro></the-intro>
    <the-body></the-body>
  </div>
  <the-footer></the-footer>
</template>

<script>
import TheIntro from "./components/layout/TheIntro.vue";
import TheBody from "./components/layout/TheBody.vue";
import TheFooter from "./components/layout/TheFooter.vue";

export default {
  components: {
    TheIntro,
    TheBody,
    TheFooter,
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
body {
  background-color: #eeeeee;
}

.container {
  width: 100%;
  max-width: 1450px;
  height: fit-content;
  margin: 10px auto;
  padding: 10px;
  display: grid;
  grid-template-columns: 2fr 4fr;
  column-gap: 25px;
}
</style>
