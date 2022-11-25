<script>
export default {
  name: "AppFooter",
};
</script>

<template>
  <section class="footer-top">
    <div class="container"></div>
  </section>
  <section class="footer-bottom">
    <div class="container">
      <div class="col-left">
        <button class="btn-sign">SIGN-UP NOW!</button>
      </div>
      <div class="col-right">
        <span>FOLLOW US</span>
        <img src="../assets/img/footer-facebook.png" />
        <img src="../assets/img/footer-twitter.png" />
        <img src="../assets/img/footer-youtube.png" />
        <img src="../assets/img/footer-pinterest.png" />
        <img src="../assets/img/footer-periscope.png" />
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.footer-top {
  height: 400px;
  background-image: url(../assets/img/footer-bg.jpg);
  background-size: cover;
  .container {
    background-image: url(../assets/img/dc-logo-bg.png);
    height: 100%;
    background-repeat: no-repeat;
    background-position: right;
  }
}
.footer-bottom {
  background-color: #303030;
  padding: 20px 20px;
  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .btn-sign {
    border-color: #0282f9;
    padding: 15px;
    background-color: #303030;
    color: white;
  }
  span {
    color: #0282f9;
  }
  .col-right {
    display: flex;
    align-items: center;
  }
  img {
    padding: 20px;
  }
}
</style>
