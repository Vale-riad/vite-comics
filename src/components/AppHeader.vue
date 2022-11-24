<script>
import AppLogo from './AppLogo.vue';
export default {
  name: 'AppHeader',
  components: {
    AppLogo
  },
  
  data() {
    return {
        links: [
            'CHARACTERS',
            'COMICS',
            'MOVIES',
            'TV',
            'GAMES',
            'COLLECTIBILES',
            'VIDEOS',
            'FANS',
            'NEWS',
            'SHOP',
        ]
    }
  }
}
</script>

<template>
  <header class="container">
    <AppLogo/>
      <nav class="main-nav">
          <ul>
              <li v-for="link in links"><a href="">{{link}}</a></li>
          </ul>
      </nav>
  </header>
</template>

<style lang="scss" scoped>
header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding:20px;
    img{
      height: 70px;
    }
    .main-nav {
        ul {
            display: flex;
            list-style: none;
            justify-content: center;
            a {
                display: inline-block;
                padding: 15px 25px;
                text-decoration: none;
                color: #000;
                font-size: 13px;
                &.active {
                    background-color: var(--secondary-color);
                }
            }
        }
    }
}
</style>
