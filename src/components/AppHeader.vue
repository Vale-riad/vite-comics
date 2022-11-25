<script>
import AppLogo from "./AppLogo.vue";
export default {
  name: "AppHeader",
  components: {
    AppLogo,
  },

  data() {
    return {
      links: [
        {
          text: "CHARACTERS",
          active: true,
        },
        {
          text: "COMICS",
          active: false,
        },
        {
          text: "MOVIES",
          active: false,
        },
        {
          text: "TV",
          active: false,
        },
        {
          text: "GAMES",
          active: false,
        },
        {
          text: "COLLECTIBILES",
          active: false,
        },
        {
          text: "VIDEOS",
          active: false,
        },
        {
          text: "FANS",
          active: false,
        },
        {
          text: "NEWS",
          active: false,
        },
        {
          text: "SHOP",
          active: false,
        },
      ],
    };
  },
  methods: {
    changeColor(index) {
      this.links.forEach((elm, i) => {
        if (index === i) {
          elm.active = true;
        } else {
          elm.active = false;
        }
      });
    },
  },
};
</script>

<template>
  <header class="container">
    <AppLogo />
    <nav class="main-nav">
      <ul>
        <li
          v-for="(link, index) in links"
          :class="{ active: link.active }"
          @click="changeColor(index)"
        >
          <a href="#">{{ link.text }}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  img {
    height: 70px;
    margin: 20px;
  }
  .main-nav {
    min-height: 110px;
    ul {
      display: flex;
      list-style: none;
      justify-content: center;
      height: 110px;
      li {
        min-height: 100%;
        margin: 0 25px;
        &.active {
          color: #0282f9;
          border-bottom: 3px solid #0282f9;
        }
      }
      a {
        display: inline-block;
        text-decoration: none;
        color: inherit;
        font-size: 13px;
        line-height: 110px;
      }
    }
  }
}
</style>
