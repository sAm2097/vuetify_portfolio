<template>
    <v-footer>
      <v-card elevation="0" rounded="0" width="100%" class="bg-grey text-center">
        <v-card-text>
          <a href="#" target="_blank" rel="noopener noreferrer">
            <v-btn class="mx-4" icon="fa-brands fa-linkedin fa-beat" variant="plain" :color="iconColor.linkedin" ></v-btn>
          </a>
          
          <a href="https://github.com/sAm2097" target="_blank" rel="noopener noreferrer">
            <v-btn class="mx-4" icon="fa-brands fa-github fa-flip" variant="plain" :color="iconColor.github"></v-btn>
          </a>
          
          <a href="#" target="_blank" rel="noopener noreferrer">
            <v-btn class="mx-4" icon="fa-brands fa-square-instagram fa-bounce" variant="plain" :color="iconColor.instagram"></v-btn>
          </a>
          
          <a href="#" target="_blank" rel="noopener noreferrer">
            <v-btn class="mx-4" icon="fa-brands fa-square-facebook fa-shake" variant="plain" :color="iconColor.facebook"></v-btn>
          </a>
        </v-card-text>
        <v-card-text class="text-white">
          @ {{ new Date().getFullYear() }} —
          <strong>All Rights Reserved</strong>
        </v-card-text>
      </v-card>
    </v-footer>
  </template>
  
  <script>
  export default {
    data() {
      return {
        iconColor: {
          linkedin: 'blue',
          github: 'black',
          instagram: '#C13584',
          facebook: 'rgb(30, 48, 80)',
        },
       
      };
    },
    methods: {
      updateIconColor(icon) {
        if (this.iconColor[icon] === this.darkerColor[icon]) {
          this.iconColor[icon] = this.originalColor[icon];
        } else {
          this.iconColor[icon] = this.darkerColor[icon];
        }
      },
    },
  };
  </script>
  
  <style>
  .v-footer {
    padding: 8px 0 !important;
  }
  a .v-btn {
   
    text-shadow: 2px 2px 2px rgba(0, 0, 0, 0.5);
  }
  </style>
  
