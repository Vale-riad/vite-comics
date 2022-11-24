<script>
import MainLogo from './MainLogo.vue';
export default {
  name: 'AppMain',
  components: {
    MainLogo
  },
}
</script>

<template>
  <main>
    <div class="background-color">
        <h1 class="container">Content goes here</h1>
    </div>
    <div class="main-top">
        <section class="container">
            <MainLogo/>
        </section>
    </div>
  </main>
</template>

<style lang="scss" scoped>
.background-color{
    background-color: black;
}
    h1{
        color: white;
        padding:30px;
    }

    .main-top{
        background-color: #0282f9;
        .container{
            display: flex;
            justify-content: space-between;
            padding:30px;
        }
    }


</style>