<template>
  <div id="app">
    <TheHeader :navbar="navbar"></TheHeader>
    <TheMain :projects="projects"></TheMain>
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
      projects: [
        {
          title: "The Basket Of Flowers",
          description: "BRANDING",
          description1: "MARKETING",
          image: "ina-soulis-227104-unsplash-1024x1024.jpg",
        },
        {
          title: "A Famous Ferris Wheel",
          description: "MARKETING",
          description1: "",
          image: "355H-1024x1024.jpg",
        },
        {
          title: "Complementary Colors",
          description: "BRANDING",
          description1: "MARKETING",
          image: "sunisa-misa-531163-unsplash-1024x1024.jpg",
        },
        {
          title: "Business Prestige",
          description: "BRANDING",
          description1: "",
          image: "photo-1448932252197-d19750584e56-1024x1024.jpg",
        },
        {
          title: "Colorful Origami Boats",
          description: "BRANDING",
          description1: "MARKETING",
          image: "business-competition-PB366D8-1024x1024.jpg",
        },
        {
          title: "Modern Couch",
          description: "",
          description1: "MARKETING",
          image: "cozy-sofa-in-living-room-PQR5AB9-1024x1024.jpg",
        },
        {
          title: "Hot Air Baloons",
          description: "BRANDING",
          description1: "MARKETING",
          image: "aa9a4539-PQGJ7HU-1024x1024.jpg",
        },
        {
          title: "Make Difference",
          description: "BRANDING",
          description1: "",
          image: "cody-davis-253928-unsplash-1024x1024.jpg",
        },
      ]
    }

  },
}


</script>

<style lang="scss">
@import "assets/scss/main.scss";
</style>
