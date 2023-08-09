<template>
  <v-col cols="12" class="padd" id="certification">
    <div class="text-center mt-4">
        <h2>My Certifications</h2>
        <div style="width: 120px; margin: 0 auto">
          <v-slider v-model="slider2" color="yellow"></v-slider>
        </div>
      </div> 
      <div class="first" ></div>
      <v-row>
        <v-col cols="12" class="imgHover">
        <v-row class="fill-height" align-items="center" justify="center">
          <template v-for="(item, i) in items" :key="i">
            <v-col cols="12" md="4">
              <v-hover v-slot="{ isHovering, props }">
                <v-card
                  :elevation="isHovering ? 12 : 2"
                  :class="{ 'on-hover': isHovering }"
                  v-bind="props"
                >
                  <v-img :src="item.img" @click="openLink(item.link)" cover> 
                <v-link ></v-link>
                </v-img>
                  <v-card-subtitle class="font-weight-black"> {{ item.title }}</v-card-subtitle>
                </v-card>
              </v-hover>
            </v-col>
          </template>
        </v-row>
      </v-col>
      <v-col cols="12" sm="12">
        <div class="d-flex justify-center mb-6">
          <v-btn color="#FBDF7E" class="mt-4">Load More</v-btn>
        </div>
      </v-col>
      </v-row>
  </v-col>
</template>

<script>
export default {
    setup() {
    return {
      slider2: 50,

      items: [
      
        {
          img: "Frontend Development.jpg",
          title:"Introduction to Front-End Development",
          link:"https://www.coursera.org/account/accomplishments/certificate/53EJFUH788PU"
        },
        {
          img: "javascript.jpg",
          title:'Programming with JavaScript',
          link:'https://www.coursera.org/account/accomplishments/certificate/HUL3D7VS6FDA'

        },
        {
          img: "vue.jpg",
          title:"Introduction to VueJS Framework",
          link:'https://www.coursera.org/account/accomplishments/certificate/U64C77CGETR2'
        },
        {
          img: "Angular.jpg",
          title:"Angular for Front End Engineers",
          link:'https://www.coursera.org/account/accomplishments/certificate/4W2T4U28G6VY'

        },
       
      ],
    };
  },
  methods: {
    openLink(link) {
      // Redirect to the link when image is clicked
      window.open(link, "_blank"); // Opens link in a new tab/window
    }
  }
}
</script>

<style>
.first {
  width: 100%;
  padding: 2rem;
}
.imgHover {
  padding: 0 200px;
}
</style>