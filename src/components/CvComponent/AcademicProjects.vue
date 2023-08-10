<template>
    <v-card >
      <v-card-title>Academic Research and Projects</v-card-title>
      <v-card-title>
        <v-icon class="mr-2">fa-solid fa-book-open-reader</v-icon>
        <span class="text-subtitle-1"> Research</span>
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
                  <span>location</span>
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
                  <span class="info">December - March </span>
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
              
            </v-list-item-group>
          </v-list>
        </v-card-text>
      </v-expand-transition>
    </v-card>
    
      
    <v-card class="mt-4">
      <v-card-title>
        <v-icon class="mr-2">fa-solid fa-code</v-icon>
        <span class="text-subtitle-1"> Project</span>
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
                  <span> India</span>
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
                  <span class="info">September  - January </span>
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
             
            </v-list-item-group>
          </v-list>
        </v-card-text>
      </v-expand-transition>
    </v-card>
    
    <v-card class="mt-4 font-italic text-body-3 text-center">
        <span>Find some of my latest projects on <a href="#" target="_black"> Github</a> </span>
    </v-card>
  </template>
  
  <script>
  export default {
    data() {
      return {
        isExpanded: false,
        isExpanded1: false,
        isExpanded2: false,
        isExpanded3: false,

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
  
