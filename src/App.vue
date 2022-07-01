<template>
  <div id="app">
    <TheHeader :navbar="navbar"></TheHeader>
    <TheMain></TheMain>
    <TheFooter></TheFooter>

  </div>
</template>

<script>

import TheHeader from './components/TheHeader.vue'
import TheMain from './components/TheMain.vue'
import TheFooter from './components/TheFooter.vue'


export default {
  name: 'App',
  components: {
    TheHeader,
    TheMain,
    TheFooter,
  },
  data() {

    return {
      navbar: ["HOME", "ABOUT", "SERVICES", "SHOWCASE", "BLOG", "CONTACT"],
    };
  },

}
</script>

<style lang="scss">
@import "assets/scss/main.scss";
</style>
