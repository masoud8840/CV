<template>
  <section class="container-fluid">
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
        content="+98 937 0700 162"
        iconHRef="fas fa-mobile-alt"
      ></contact-item>
    </div>
  </section>
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

section.container-fluid {
  width: 100%;
  display: flex;
  flex-direction: column;

  .user-profile {
    height: 300px;
    background: url("../../assets/profile.jpg") center no-repeat;
    background-size: contain;
    @include Flexbox(flex-end, flex-start, column);
    padding: 20px 10px;

    p {
      color: #757575;
    }
  }
}
</style>