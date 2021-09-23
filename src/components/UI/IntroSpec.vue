<template>
  <div class="container">
    <div class="user-profile">
      <h1>Masoud Gharedaghi</h1>
      <p>Web Designer</p>
    </div>
    <div class="user-contact">
      <contact-item content="Tehran, IR" iconHRef="fas fa-home"></contact-item>
      <contact-item
        content="gharedaghi.zip@gmail.com"
        iconHRef="fas fa-envelope"
      ></contact-item>
      <contact-item
        content="Tehran, IR"
        iconHRef="fas fa-mobile-alt"
      ></contact-item>
    </div>
  </div>
</template>



<script>
import ContactItem from "./UIComponents/ContactItem.vue";

export default {
  components: {
    ContactItem,
  },
};
</script>


<style lang="scss" scoped>
@mixin Flexbox($justify, $align, $dir) {
  display: flex;
  justify-content: $justify;
  align-items: $align;
  flex-direction: $dir;
}

.container {
  width: 100%;
  height: 400px;
  display: flex;
  flex-direction: column;
  .user-profile {
    height: 300px;
    background: url("../../assets/logo.png") center no-repeat;
    @include Flexbox(flex-end, flex-start, column);
    background-color: lime;
    padding: 20px 10px;
  }
}
</style>