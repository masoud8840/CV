<template>
  <section>
    <div class="icon">
      <i :class="iconHRef"></i>
    </div>
    <div class="txt">
      <p>{{ content }}</p>
    </div>
  </section>
</template>


<script>
export default {
  props: ["content", "iconHRef"],
};
</script>

<style lang="scss" scoped>
@mixin Flexbox($justify, $align, $dir) {
  display: flex;
  justify-content: $justify;
  align-items: $align;
  flex-direction: $dir;
}
section {
  width: 100%;
  @include Flexbox(flex-start, center, row);
  margin: 10px 0;
  .icon {
    width: 40px;
    @include Flexbox(center, center, row);
    i {
      color: #009688;
      font-size: 20px;
    }
  }
  .txt {
    p {
      color: #757575;
      font: 400 15px Roboto;
    }
  }
}
</style>