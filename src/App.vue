<template>
  <div id="app">
    <Header :links="headerMenu" />
    <Main />
    <Footer :links="headerMenu" />
  </div>
</template>

<script>
import Header from "./components/HeaderComponent.vue";
import Main from "./components/MainComponent.vue";
import Footer from "./components/FooterComponent.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
  data() {
    return {
      headerMenu: [
        "CHARACTERS",
        "COMICS",
        "MOVIES",
        "TV",
        "GAMES",
        "COLECTIBLES",
        "VIDEOS",
        "FANS",
        "NEWS",
        "SHOP",
      ],
    };
  },
};
</script>

<style lang="scss">
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
ul {
  list-style-type: none;
}
li {
  padding: 0px 10px;
  display: inline;
}
.c-grey {
  color: grey;
}
.c-white {
  color: white !important;
}
a {
  text-decoration: none !important;
}
</style>
