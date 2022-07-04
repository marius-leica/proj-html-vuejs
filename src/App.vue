<template>
  <div id="app">
    <TheHeader :navbar="navbar"></TheHeader>
    <TheMain></TheMain>
    <TheFooter :quick-links="quickLinks" :contact="contact"></TheFooter>

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
      quickLinks: ["Careers", "News", "Terms of use", "Privacy Projects", "About", "Contacts"],
      contact: ["Patricia C. Amedee 4401 Waldeck Street Grapevine Nashville, TX 76051", "info@yourdomain.com", "+99(0)1010000888"],

    };
  },

}
</script>

<style lang="scss">
@import "assets/scss/main.scss";
</style>
