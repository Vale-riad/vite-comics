<script>
import MainLogo from "./MainLogo.vue";
import SectionCard from "./SectionCard.vue";
export default {
  name: "AppMain",
  components: {
    MainLogo,
    SectionCard,
  },
};
</script>

<template>
  <main>
    <div class="hero"></div>
    <div class="background-color">
      <div class="container">
        <SectionCard />
      </div>
    </div>
    <div class="main-bottom">
      <section class="container">
        <MainLogo />
      </section>
    </div>
  </main>
</template>

<style lang="scss" scoped>
.hero {
  background-image: url(../assets/img/jumbotron.jpg);
  height: 400px;
  background-size: cover;
  background-repeat: no-repeat;
}
.background-color {
  background-color: #1c1c1c;
}
h1 {
  color: white;
  padding: 30px;
}

.main-bottom {
  background-color: #0282f9;
  .container {
    display: flex;
    justify-content: space-between;
    padding: 30px;
  }
}
</style>
