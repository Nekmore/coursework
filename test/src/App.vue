<template>
  <div id="main">
    <Head />
    <Menu />
    <Main />

  </div>

</template>

<script>

import Main from "./components/Main";
import Head from "./components/Head";
import Menu from "@/components/Menu";


export default {
  components: {Menu, Main, Head},
  data() {
    return {

    }
  }
}
</script>

<style>
  * {
    font-family: "Montserrat", sans-serif;
  }

  body {
    overflow-x: hidden;
  }
</style>
