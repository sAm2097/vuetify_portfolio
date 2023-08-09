<template>
  <v-app-bar app color="black" dark flat class="px-12">
    <v-btn app icon @click="isMenuOpen = !isMenuOpen" v-if="isMobile">
      <v-icon>fas fa-bars</v-icon>
    </v-btn>
    <v-toolbar-title>
      <v-btn>
        <v-icon color="blue" left class="mr-2">fas fa-signature</v-icon> Mr. A
      </v-btn>
    </v-toolbar-title>
    <v-spacer></v-spacer>

    <v-btn text @click="scroll('home')" class="text-blue" v-show="!isMobile">Home</v-btn>
    <v-btn text @click="scroll('about')" v-show="!isMobile">About</v-btn>
    <v-btn text @click="scroll('portfolio')" v-show="!isMobile">Portfolio</v-btn>
    <!-- <v-btn text @click="scroll('services')" v-show="!isMobile"> Services</v-btn> -->
    <router-link to="/curriculam_vitae" class="text-white" v-show="!isMobile">
      <v-btn text>CV</v-btn>
    </router-link>
    <v-btn text @click="scroll('certification')" v-show="!isMobile">certifications</v-btn>
    <v-btn text @click="scroll('contact')" v-show="!isMobile">Contact</v-btn>

    <v-menu v-model="isMenuOpen" offset-y>
      <v-list>
        <v-list-item @click="scroll('home')">
          <v-list-item-title>Home</v-list-item-title>
        </v-list-item>
        <v-list-item @click="scroll('about')">
          <v-list-item-title>About</v-list-item-title>
        </v-list-item>
        <v-list-item @click="scroll('portfolio')">
          <v-list-item-title>Portfolio</v-list-item-title>
        </v-list-item>
        <v-list-item to="/curriculam_vitae" >
          <v-list-item-title>CV</v-list-item-title>
        </v-list-item>
        <v-list-item @click="scroll('certification')">
          <v-list-item-title>certifications</v-list-item-title>
        </v-list-item>
        <v-list-item @click="scroll('contact')">
          <v-list-item-title>Contact</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-menu>
  </v-app-bar>
</template>

<script>
export default {
  data() {
    return {
      isMenuOpen: false,
      isMobile: false,
    };
  },
  methods: {
    scroll(refName) {
      const element = document.getElementById(refName);
      if (element) {
        element.scrollIntoView({ behavior: "smooth" });
        this.isMenuOpen = false;
      }
    },
  },
  created() {
    // Check if it's a mobile device (width <= 600px)
    this.isMobile = window.innerWidth <= 600;
    // Listen for window resize to update isMobile value
    window.addEventListener("resize", () => {
      this.isMobile = window.innerWidth <= 600;
    });
  },
};
</script>
