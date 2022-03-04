<template>
  <section class="container-fluid">
    <div class="user-profile">
      <h1>Masoud Gharedaghi</h1>
      <p>Web Developer</p>
    </div>
    <div class="user-contact">
      <contact-item content="Tehran, IR" iconHRef="fas fa-home"></contact-item>
      <contact-item
        content="03-05-2001"
        iconHRef="fas fa-calendar-plus"
      ></contact-item>
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
    height: 350px;
    background: transparent url("../../assets/profile.png") center/cover
      no-repeat;
    @include Flexbox(flex-end, flex-start, column);
    padding: 20px 20px;

    h1 {
      color: #fafafa;
      font: 400 26px "Roboto";
    }

    p {
      color: #e2e2e2;
      font: 400 16px "Roboto";
      margin-top: 0px;
    }
  }
  .user-contact {
    padding: 0 10px;
  }
}
</style>
