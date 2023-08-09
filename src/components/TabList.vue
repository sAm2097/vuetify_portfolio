<template>
  <v-card>
    <v-tabs v-model="activeTab" background-color="primary">
      <v-tab v-for="(tab, index) in tabList" :key="index" :value="index">
        <v-icon>
          {{ tabIcons[index] }}
        </v-icon>
      </v-tab>
    </v-tabs>

    <v-card-text>
      <v-window v-model="activeTab">
        <v-window-item
          v-for="(tab, index) in tabList"
          :key="index"
          :value="index"
        >
          <component :is="getComponentName(index)"></component>
        </v-window-item>
      </v-window>
    </v-card-text>
  </v-card>
</template>

<script>
import PersonalDetails from "@/components/CvComponent/PersonalDetails.vue";
import ExperienceComp from "@/components/CvComponent/ExperienceComp.vue";
import EducationalDetails from "@/components/CvComponent/EducationalDetails.vue";
import AcademicProjects from "@/components/CvComponent/AcademicProjects.vue";
import AllSkills from "@/components/CvComponent/AllSkills.vue";

export default {
  data() {
    return {
      activeTab: 0,
      tabList: [
        "Personal Info",
        "Experience",
        "Education",
        "Projects",
        "Skills",
      ],
      tabIcons: [
        "fas fa-user",
        "fas fa-briefcase",
        "fas fa-graduation-cap",
        "fas fa-project-diagram",
        "fas fa-tools",
      ],
    };
  },
  components: {
    PersonalDetails,
    ExperienceComp,
    EducationalDetails,
    AcademicProjects,
    AllSkills,
  },
  methods: {
    getComponentName(index) {
      const components = [
        "PersonalDetails",
        "ExperienceComp",
        "EducationalDetails",
        "AcademicProjects",
        "AllSkills",
      ];
      return components[index];
    },
  },
};
</script>

<style scoped></style>
