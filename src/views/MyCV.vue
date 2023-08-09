<template>
  <v-app>
    <v-app-bar app color="black" dark flat class="px-12">
      <v-btn @click="this.$router.push({name:'home'})">
        <v-icon color="blue" left class="mr-2" >fas fa-signature</v-icon> Mr. A
      </v-btn>
      <v-spacer></v-spacer>
      <router-link
        to="/"
        class="text-blue"
        style="
           {
            text-decoration: none;
          }
        "
        >Home</router-link
      >
    </v-app-bar>
   

    <v-container fluid class="my-6 mt-15">
      <v-row>
        <v-col cols="12">
          <TabList />
        </v-col>
      </v-row>
    </v-container>
    <TheFooter class="footer"></TheFooter>
  </v-app>
</template>

<script>
import TheFooter from "../components/TheFooter.vue";
import TabList from '@/components/TabList.vue'
export default {
  components: {
    TheFooter,
    TabList
  },
  data(){
    return {
        activeTab: null, // Set the initial active tab
        tabList: ['Personal Info', 'Experience','Education',  'Projects', 'Skills'],
    }
  }
};
</script>

<style>
.footer {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  height: 50px; /* Adjust the height according to your footer content */
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #f5f5f5;
}
.my-6 {
  margin-top: 6rem;
  margin-bottom: 6rem;
}
</style>








