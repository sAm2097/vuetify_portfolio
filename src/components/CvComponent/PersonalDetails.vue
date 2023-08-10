<template>
    <v-card>
      <v-card-title>Personal Information</v-card-title>
      <v-card-text>
        <v-row>
          <v-col cols="12" md="6">
            <v-row>
              <v-col cols="2">
                <v-icon class="mr-2">fas fa-user</v-icon>
              </v-col>
              <v-col cols="10">
                <span> Name</span>
              </v-col>
            </v-row>
          </v-col>
          <v-col cols="12" md="6">
            <v-row>
              <v-col cols="2">
                <v-icon class="mr-2">fas fa-envelope</v-icon>
              </v-col>
              <v-col cols="10">
                <span>example@gmail.com</span>
              </v-col>
            </v-row>
          </v-col>
          <v-col cols="12" md="6">
            <v-row>
              <v-col cols="2">
                <v-icon class="mr-2">fas fa-phone</v-icon>
              </v-col>
              <v-col cols="10">
                <span> +49 xxx xxx xxxx</span>
              </v-col>
            </v-row>
          </v-col>
          <v-col cols="12" md="6">
            <v-row>
                <v-col cols="2">
                    <v-icon class="mr-2">fa fa-location-dot</v-icon>
                </v-col>
                <v-col cols="10">
                    <span>Location</span>
                </v-col>
            </v-row>
          </v-col>
          <v-col cols="12" md="6">
            <v-row>
                <v-col cols="2">
                    <v-icon class="mr-2">fa fa-cake-candles</v-icon>
                </v-col>
                <v-col cols="10">
                    <span>DOB</span>
                </v-col>
            </v-row>
          </v-col>
        </v-row>
      </v-card-text>
    </v-card>
  </template>
  
  <script>
  export default {
    // Component logic and properties
  }
  </script>
  
  <style scoped>
  /* Component-specific styles */
  </style>
  
