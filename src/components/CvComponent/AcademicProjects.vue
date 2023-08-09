<template>
    <v-card >
      <v-card-title>Academic Research and Projects</v-card-title>
      <v-card-title>
        <v-icon class="mr-2">fa-solid fa-book-open-reader</v-icon>
        <span class="text-subtitle-1"> Research on Car2Car Communication Applications</span>
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
                  <span class="info">December2020 - March 2021</span>
                </v-col>
              </v-row>
            </v-cols>
          </v-row>
  
          <v-list class="mt-5 dotted-list">
            <v-list-item-group>
              <v-list-item>
                <v-list-item-content>
                    Researched V2V communication systems in Europe, America, and Japan.
                </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content>
                    Created a technical report on V2V applications and their pros and cons.
                </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content>
                    Identified best practices for V2V communication based on industry standards.
                </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content>
                    Wrote a comprehensive report for both technical and non-technical readers.
                </v-list-item-content>
              </v-list-item>
            </v-list-item-group>
          </v-list>
        </v-card-text>
      </v-expand-transition>
    </v-card>
    <v-card class="mt-4">
      <v-card-title>
        <v-icon class="mr-3">fa-solid fa-book-open-reader</v-icon>
        <span class="text-subtitle-1">Research on Car2X Communication Protocols</span>
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
                  <span class="info">April2020 - July 2020</span>
                </v-col>
              </v-row>
            </v-cols>
          </v-row> 
          <v-list class="mt-5 dotted-list">
            <v-list-item-group>
              <v-list-item>
                <v-list-item-content>
                    Researched and analyzed various. Car2X protocols including European, American, and Japanese systems.
                </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content>
                    Compared WAVE with ITS-G5 and ARIB standards.
                </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content>
                    Created a seminar report with 18 technical references to showcase the differences and advantages of each protocol.
                </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content>
                    Wrote a clear and concise report that effectively conveys the research results to both technical and non-technical audiences.
                </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content>
                    Delivered a successful presentation of the research findings to an audience of professors and colleagues.
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
        <span class="text-subtitle-1"> Image Processing and Machine Learning for Precision Viticulture</span>
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
                  <span>Malla Reddy Engieering College, Hyderabad, India</span>
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
                  <span class="info">September 2018 - January 2019</span>
                </v-col>
              </v-row>
            </v-cols>
          </v-row> 
          <v-list class="mt-5 dotted-list">
            <v-list-item-group>
              <v-list-item>
                <v-list-item-content>
                    Predicted grape variety with 95 % accuracy using a deep learning model trained on 1,000 grape images in Python and TensorFlow.
                </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content>
                    Applied image processing techniques such as resizing and normalization to improve the model's accuracy on a dataset of 1,000 grape images.
                </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content>
                    Developed and fine-tuned a 5-layer CNN model to achieve high accuracy in predicting grape varieties.
                </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content>
                    Conducted hyperparameter tuning and optimization by adjusting the learning rate and number of epochs to obtain optimal results.
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
        <span class="text-subtitle-1"> Query Handling System</span>
        <v-btn
          icon
          @click="isExpanded3 = !isExpanded3"
          class="ml-6"
          size="x-small"
        >
          <v-icon variant="plain">{{
            isExpanded3 ? "fas fa-chevron-up" : "fas fa-chevron-down"
          }}</v-icon>
        </v-btn>
      </v-card-title>
      <v-expand-transition>
        <v-card-text v-if="isExpanded3" class="scrollable-content">
          <v-row class="mt-3">
            <v-cols cols="12" md="6">
              <v-row>
                <v-col cols="2">
                  <v-icon class="mr-2">fa fa-location-dot</v-icon>
                </v-col>
                <v-col cols="8">
                  <span>Malla Reddy Engieering College, Hyderabad, India</span>
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
                  <span class="info">April 2018 - June 2018</span>
                </v-col>
              </v-row>
            </v-cols>
          </v-row> 
          <v-list class="mt-5 dotted-list">
            <v-list-item-group>
              <v-list-item>
                <v-list-item-content>
                    Developed a web application for 500+ students using HTML, CSS, and JavaScript.
                </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content>
                    Created an online forum to enhance communication between students and faculty.
                </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content>
                    Reduced average response time by 30 % through the online forum.
                </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content>
                    Conducted user testing and incorporated feedback to improve functionality.
                </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content>
                    Increased user engagement by 40 % through the implemented improvements.
                </v-list-item-content>
              </v-list-item>
            </v-list-item-group>
          </v-list>
        </v-card-text>
      </v-expand-transition>
    </v-card>

    <v-card class="mt-4 font-italic text-body-3 text-center">
        <span>Find some of my latest projects on <a href="https://github.com/sAm2097" target="_black"> Github</a> </span>
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
  