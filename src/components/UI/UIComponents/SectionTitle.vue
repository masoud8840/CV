<template>
  <div class="title">
    <div class="icon">
      <i :class="classHRef"></i>
    </div>
    <div class="txt">
      <h2>{{ content }}</h2>
    </div>
  </div>
</template>
<script>
export default {
  props: ["classHRef", "content"],
};
</script>
<style lang="scss" scoped>
@mixin Flexbox($justify, $align, $dir) {
  display: flex;
  justify-content: $justify;
  align-items: $align;
  flex-direction: $dir;
}

.title {
  width: 100%;
  height: 60px;
  display: flex;
  .icon {
    width: 70px;
    height: 100%;
    @include Flexbox(flex-start, center, row);
    padding: 0 0 0 20px;
    i {
      color: #009688;
      font-size: 28px;
      padding: 3px 0 0 0;
    }
  }
  .txt {
    @include Flexbox(flex-start, center, row);
    h2 {
      font: 700 24px Roboto;
      color: #757575;
    }
  }
}
</style>