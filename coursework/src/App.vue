<template>
  <div id="main">
    <Head v-if="!isMobile"/>
    <Menu v-if="!isMobile"/>
    <MenuMobile v-if="isMobile" />
    <Main />
  </div>

</template>

<script>

import Main from "./components/Main";
import Head from "./components/Head";
import Menu from "@/components/Menu";
import MenuMobile from "@/components/MenuMobile"

export default {
  components: {Menu, Main, Head, MenuMobile},
  data() {
    return {
        width: null,
        isMobile: window.innerWidth < 1280,
    }
  },
  methods: {
  updateWidth() {
      this.width = window.innerWidth;
      this.isMobile = this.width < 1280;
    },
  },
  created() {
    window.addEventListener('resize', this.updateWidth);
    this.updateWidth();
  },

}
</script>

<style>
  * {
    font-family: "Montserrat", sans-serif;

  }

  body {
    overflow-x: hidden;
    margin-top: 0;
  }
</style>
