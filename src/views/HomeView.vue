<template>
  <v-app id="home">
    <NavBar></NavBar>
    <v-container class="container" fluid>
      <HomeComp></HomeComp>
     
      <AboutView></AboutView>
      <div class="section-divider"></div>
      <ThePortfolio></ThePortfolio>
      <div class="section-divider">
        <CertificationComp></CertificationComp>
      </div>
      <div class="section-divider"></div>
      <ContactComp></ContactComp>
      
    </v-container>
    <TheFooter></TheFooter>
  </v-app>
</template>

<script>
import { defineComponent } from "vue";
import NavBar from "../components/NavBar.vue";
import TheFooter from "../components/TheFooter.vue";
import AboutView from "../views/AboutView.vue";
import ContactComp from "../components/ContactComp.vue";
import ThePortfolio from "@/components/ThePortfolio.vue";
import HomeComp from "@/components/HomeComp.vue";
import CertificationComp from '@/components/CertificationComp.vue'

// Components

export default defineComponent({
  name: "HomeView",

  components: {
    NavBar,
    TheFooter,
    AboutView,
    ContactComp,
    ThePortfolio,
    HomeComp,
    CertificationComp
  },
});
</script>

<style scoped>
.container {
  padding: 16px 0;
  overflow-y: auto;
  scrollbar-color: transparent transparent; /* For Firefox */
  -ms-overflow-style: none; /* For Internet Explorer and Edge */
  scrollbar-width: none; /* For Internet Explorer and Edge */
}

.container::-webkit-scrollbar {
  width: 0;
  background-color: transparent;
}

.container::-webkit-scrollbar-thumb {
  background-color: transparent;
}
.section-divider {
  border-top: 1px solid #e0e0e0;
  margin-top: 2rem;
  margin-bottom: 2rem;
}
</style>
