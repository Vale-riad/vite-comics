<script>
export default {
  name: 'MainLogo',
}
</script>
<template>
    <div>
      <img src="../assets/img/buy-comics-digital-comics.png">
      <span>Digital Comics</span>
    </div>
    <div>
      <img src="../assets/img/buy-comics-merchandise.png">
      <span>DC Merchandise</span>
    </div>
    <div>
      <img src="../assets/img/buy-comics-shop-locator.png">
      <span>Subscription</span>
    </div>
    <div>
      <img src="../assets/img/buy-comics-subscriptions.png">
      <span>Comic shop locator</span>
    </div>
    <div>
      <img src="../assets/img/buy-dc-power-visa.svg">
      <span>Dc power visa</span>
    </div>
  </template>
  
  <style lang="scss" scoped>
  img{
    max-width: 50px;
    max-height:50px;
  }
  span{
    padding:10px;
    color:white;
  }
  div{
    display: flex;
    align-items: center;
  }
  </style>