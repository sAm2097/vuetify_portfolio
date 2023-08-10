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
                <span>Company</span>
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
                <span class="info">Duration</span>
              </v-col>
            </v-row>
          </v-cols>
        </v-row>

        <v-list class="mt-5 dotted-list">
          <v-list-item-group>
            <v-list-item>
              <v-list-item-content>
                detail...
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
               detail...
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
              detail...
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
      <span class="text-subtitle-1"> Position</span>
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
                <span>company</span>
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
                <span class="info">duration</span>
              </v-col>
            </v-row>
          </v-cols>
        </v-row>

        <v-list class="mt-5 dotted-list">
          <v-list-item-group>
            <v-list-item>
              <v-list-item-content>
detail...
                Learning Scenario.
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
               detail...
                software.
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
             
                realism and user engagement.
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
              
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
