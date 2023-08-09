<template>
     <v-card>
        <v-card-title>Academics</v-card-title>
    <v-card-title>
      
        <v-icon class="mr-2">fa-solid fa-building-columns</v-icon>
      <span class="text-subtitle-1"> Master's in Automotive Software Engineering</span>
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
                <span class="info">October 2019 - August 2022</span>
              </v-col>
            </v-row>
          </v-cols>
        </v-row>

        <v-list class="mt-5 dotted-list">
          <v-list-item-group>
            Focused Modules:
            <v-list-item>
              <v-list-item-content>
                Automotive Software Technology 
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Computer Science
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Real-time and Communication Systems
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Embedded Systems
              </v-list-item-content>
            </v-list-item>
            Learned about:
            <v-list-item>
              <v-list-item-content>
                Real-time operating systems 
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Communication protocols
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Software architectures
              </v-list-item-content>
            </v-list-item>
          </v-list-item-group>
        </v-list>
      </v-card-text>
    </v-expand-transition>
  </v-card>

  <v-card class="mt-4">
    <v-card-title>
        <v-icon class="mr-2">fa-solid fa-building-columns</v-icon>
      <span class="text-subtitle-1"> Bachelor's in Computer Science and Engineering</span>
      <v-btn icon @click="isExpanded1 = !isExpanded1" class="ml-6" size="x-small">
        <v-icon>{{
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
                <span>Malla Reddy Engineering College, Hyderabad, India</span>
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
                <span class="info">September 2015 - April 2019</span>
              </v-col>
            </v-row>
          </v-cols>
        </v-row>

        <v-list class="mt-5 dotted-list">
          <v-list-item-group>
            Skills Developed:
            <v-list-item>
              <v-list-item-content>
                Foundation in programming languages, algorithms, data structures, database systems, computer networks, and software engineering modules
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Solid foundation in programming and problem-solving skills
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Emphasis on developing soft skills such as teamwork, communication, and leadership  
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Collaborated on group projects to enhance interpersonal skills
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-content>
                Equipped with a comprehensive understanding of computer science principles
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
    };
  },
  }
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