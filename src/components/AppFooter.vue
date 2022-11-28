<script>
export default {
  name: "AppFooter",
  data() {
    return {
      links: [
        "Characters",
        "Comics",
        "Movies",
        "TV",
        "Games",
        "Videos",
        "News",
      ],
      dcList: [
        "Terms Of use",
        "Privacy policy (New)",
        "Ad Choices",
        "Advertising",
        "Jobs",
        "Subscriptions",
        "Talent Workshops",
        "CPSC Certificates",
        "Ratings",
        "Shop Help",
        "Contact Us",
      ],
    };
  },
};
</script>

<template>
  <section class="footer-top">
    <div class="container">
      <div class="list-left">
        <h3>DC COMICS</h3>
        <ul>
          <li v-for="link in links">
            <a href="">{{ link }}</a>
          </li>
        </ul>
        <h3>SHOP</h3>
        <ul>
          <li><a href="#">Shop Dc</a></li>
          <li><a href="#">Shop Dc Collectibles</a></li>
        </ul>
      </div>
      <div class="list-center">
        <h3>DC</h3>
        <ul>
          <li v-for="link in dcList">
            <a href="">{{ link }}</a>
          </li>
        </ul>
      </div>
      <div class="list-right">
        <h3>SITIES</h3>
        <ul>
          <li><a href="#">Dc</a></li>
          <li><a href="#">Mad Magazine</a></li>
          <li><a href="#">DC kids</a></li>
          <li><a href="#">DC Universe</a></li>
          <li><a href="#">DC Power Visa</a></li>
        </ul>
      </div>
    </div>
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
    display: flex;
  }
  h3 {
    color: white;
    margin-top: 50px;
  }
  ul {
    list-style: none;
    a {
      text-decoration: none;
      font-size: 13px;
      padding: 15px 25px 0 0;
      color: gray;
    }
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
