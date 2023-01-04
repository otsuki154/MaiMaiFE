<template>
  <div id="app">
    <Navbar :itemMenu="initMenu" :isDisplay="isDisplay"></Navbar>
  </div>
</template>

<script>
import Navbar from "./templates/commonPages/menu.vue";

export default {
  name: "App",
  components: {
    Navbar,
  },
  data() {
    return {
      initMenu: [
        { id: 1, url: "/", name: "ホーム" },
        { id: 2, url: "/goi", name: "語彙" },
        { id: 3, url: "/kanji", name: "漢字" },
        { id: 4, url: "/grammar", name: "文法" },
        { id: 5, url: "/contact", name: "連絡先" },
        { id: 6, url: "/test", name: "機能確認専用" },
      ],
      isDisplay: true,
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
