<template>
  <v-card>
    <v-card-title>Professional Experience</v-card-title>
    <v-card-title>
      <v-icon class="mr-2">fa-solid fa-building</v-icon>
      <span class="text-subtitle-1"> Software Engineer</span>
      <v-btn icon @click="isExpanded = !isExpanded" class="ml-6" size="x-small">
        <v-icon>{{
          isExpanded ? "fas fa-chevron-up" : "fas fa-chevron-down"
        }}</v-icon>
      </v-btn>
    </v-card-title>
    <v-expand-transition>
      <v-card-text v-if="isExpanded" class="scrollable-content">
        <v-row class="mt-3">
          <v-cols cols="12" md="6">
            <v-row>
              <v-col cols="2">
                <v-icon class="mr-2">fa fa-location-dot</v-icon>
              </v-col>
              <v-col cols="10">
                <span>Hecht AG, Besigheim, Germany</span>
              </v-col>
            </v-row>
          </v-cols>
          <v-spacer></v-spacer>
          <v-cols cols="12" md="6">
            <v-row>
              <v-col cols="2">
                <v-icon class="mr-2" :size="iconSize">fas fa-calendar</v-icon>
              </v-col>
              <v-col cols="10">
                <span class="info">April 2022 - April 2023</span>
              </v-col>
            </v-row>
          </v-cols>
        </v-row>

        <v-list class="mt-5 dotted-list">
          <v-list-item-group>
            <v-list-item>
              <v-list-item-content>
                Assessed feasibility and viability of projects.
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Contributed to Frontend development project.
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Provided consulting for image processing systems.
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Enhanced image quality using GIMP software through editing and
                optimization.
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Trained images for image processing using PuTTY software.
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Utilized Git and Bitbucket for version control and efficient
                code deployment to servers.
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Translations & Documentation
              </v-list-item-content>
            </v-list-item>
          </v-list-item-group>
        </v-list>
      </v-card-text>
    </v-expand-transition>
  </v-card>
  <v-card class="mt-4">
    <v-card-title>
      <v-icon class="mr-2">fa-solid fa-building</v-icon>
      <span class="text-subtitle-1"> Thesis student</span>
      <v-btn
        icon
        @click="isExpanded1 = !isExpanded1"
        class="ml-6"
        size="x-small"
      >
        <v-icon variant="plain">{{
          isExpanded1 ? "fas fa-chevron-up" : "fas fa-chevron-down"
        }}</v-icon>
      </v-btn>
    </v-card-title>
    <v-expand-transition>
      <v-card-text v-if="isExpanded1" class="scrollable-content">
        <v-row class="mt-3">
          <v-cols cols="12" md="6">
            <v-row>
              <v-col cols="2">
                <v-icon class="mr-2">fa fa-location-dot</v-icon>
              </v-col>
              <v-col cols="10">
                <span>Chemnitz University of Technology, 09111 Chemnitz</span>
              </v-col>
            </v-row>
          </v-cols>
          <v-spacer></v-spacer>
          <v-cols cols="12" md="6">
            <v-row>
              <v-col cols="2">
                <v-icon class="mr-2" :size="iconSize">fas fa-calendar</v-icon>
              </v-col>
              <v-col cols="10">
                <span class="info">Febuary 2022 - August 2022</span>
              </v-col>
            </v-row>
          </v-cols>
        </v-row>

        <v-list class="mt-5 dotted-list">
          <v-list-item-group>
            <v-list-item>
              <v-list-item-content>
                Designed and developmented of a Virtual Agent for Interactive
                Learning Scenario.
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Created interactive male and female agents using Autodesk Maya
                software.
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Implemented support for various facial expressions, enhancing
                realism and user engagement.
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Conducted comprehensive user testing and incorporated feedback,
                resulting in an 80 % increase in user satisfaction.
              </v-list-item-content>
            </v-list-item>
          </v-list-item-group>
        </v-list>
      </v-card-text>
    </v-expand-transition>
  </v-card>
  <v-card class="mt-4 ">
    <v-card-title>
      <v-icon class="mr-2">fa-solid fa-building</v-icon>
      <span class="text-subtitle-1"> Research Intern</span>
      <v-btn
        icon
        @click="isExpanded2 = !isExpanded2"
        class="ml-6"
        size="x-small"
      >
        <v-icon variant="plain">{{
          isExpanded2 ? "fas fa-chevron-up" : "fas fa-chevron-down"
        }}</v-icon>
      </v-btn>
    </v-card-title>
    <v-expand-transition>
      <v-card-text v-if="isExpanded2" class="scrollable-content">
        <v-row class="mt-3">
          <v-cols cols="12" md="6">
            <v-row>
              <v-col cols="2">
                <v-icon class="mr-2">fa fa-location-dot</v-icon>
              </v-col>
              <v-col cols="8">
                <span>Chemnitz University of Technology, 09111 Chemnitz</span>
              </v-col>
            </v-row>
          </v-cols>
          <v-spacer></v-spacer>
          <v-cols cols="12" md="6">
            <v-row>
              <v-col cols="2">
                <v-icon class="mr-2" :size="iconSize">fas fa-calendar</v-icon>
              </v-col>
              <v-col cols="10">
                <span class="info">Nov 2020 - June 2021</span>
              </v-col>
            </v-row>
          </v-cols>
        </v-row>

        <v-list class="mt-5 dotted-list">
          <v-list-item-group>
            <v-list-item>
              <v-list-item-content>
                Optimized ETL processes with Python, reducing processing time by
                50 %.
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Achieved 95% prediction accuracy on a dataset of 10,000 records
                using supervised learning algorithms.
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Conducted thorough exploratory data analysis (EDA) with Python,
                identifying trends and patterns through 20+ visualizations.
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Developed machine learning models with 90% prediction accuracy
                on test data.
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Enhanced model performance by 30% through advanced data
                processing and feature engineering techniques.
              </v-list-item-content>
            </v-list-item>
          </v-list-item-group>
        </v-list>
      </v-card-text>
    </v-expand-transition>
  </v-card>
</template>

<script>
export default {
  data() {
    return {
      isExpanded: false,
      isExpanded1: false,
      isExpanded2: false,
    };
  },
};
</script>

<style>
.dotted-list .v-list-item__content::before {
  content: "\2022";
  margin-right: 0.5em;
  color: #888;
}
.scrollable-content {
  max-height: 200px;
  overflow-y: auto;
  overflow-x: hidden;
}
</style>
