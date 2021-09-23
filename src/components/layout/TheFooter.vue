<template>
  <footer>
    <p>find me on social media.</p>
    <div class="socialMedia">
      <a href="https://www.instagram.com/gharedaghi.ce" title="gharedaghi.ce"
        ><i class="fab fa-instagram"></i
      ></a>
      <a href="https://t.me/gharedaghi_zip" title="gharedaghi_zip"
        ><i class="fab fa-telegram-plane"></i
      ></a>
      <a href="https://www.facebook.com/ce.911"
        ><i class="fab fa-facebook-f" title="ce.911"></i
      ></a>
      <a href="https://github.com/masoud8840" title="masoud8840"
        ><i class="fab fa-github"></i
      ></a>
    </div>
    <p>Powered by Masoud Gharedaghi</p>
  </footer>
</template>
<style lang="scss" scoped>
@mixin Flexbox($justify, $align, $dir) {
  display: flex;
  justify-content: $justify;
  align-items: $align;
  flex-direction: $dir;
}
footer {
  width: 100%;
  height: 120px;
  background-color: #009688;
  @include Flexbox(space-evenly, center, column);
  p {
    color: #fafafa;
    text-transform: capitalize;
    font: 400 15px Roboto;
    &:nth-child(3) {
      font-size: 13px;
    }
  }
  .socialMedia {
    width: 100px;
    @include Flexbox(space-evenly, center, row);
    a {
      color: #fafafa;
      i {
        font-size: 19px;
      }
      &:hover {
        color: #acddda;
      }
    }
  }
}
</style>