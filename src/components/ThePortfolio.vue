<template>   
   <v-col cols="12" class="padd" id="portfolio">
    <div class="text-center mt-4">
        <h2>What I Do</h2>
        <div style="width: 120px; margin: 0 auto">
          <v-slider v-model="slider2" color="yellow"></v-slider>
        </div>
      </div>    
        <div class="first" id="project">
          <v-row>
            <v-col cols="6">
              <div class="child">
                <v-btn
                  icon="fas fa-laptop"
                  color="#FBDF7E"
                  class="text-white"
                ></v-btn>
                <h3 class="ml-3 mt-4">Web Develolpment</h3>
                <p class="text-grey ml-3 mt-4 text-caption">
                  "Crafting visually stunning and user-friendly websites that
                  leave a lasting impression. From captivating layouts to
                  seamless navigation, With a passion for creating intuitive
                  user experiences, I specialize in crafting visually stunning
                  websites that seamlessly blend aesthetics and functionality.
                  From responsive designs to captivating animations, I strive to
                  bring each client's vision to life."
                </p>
              </div>
            </v-col>
            <v-col cols="6">
              <div class="child">
                <v-btn
                  icon="fas fa-mobile-alt"
                  color="#FBDF7E"
                  class="text-white"
                ></v-btn>   
                <h3 class="ml-3 mt-4">Web/App Design</h3>
                <p class="text-grey ml-3 mt-4 text-caption">
                  "Step into my world of app design where creativity meets
                  functionality! As an experienced app designer, I am dedicated
                  to crafting intuitive interfaces that enhance user engagement.
                  From wireframing to prototyping, I bring innovative ideas to
                  reality and deliver exceptional user experiences."
                </p>
              </div>
            </v-col>
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
                  <v-img :src="item.img" height="225px" cover> </v-img>
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
        </div>
      </v-col>
</template>

<script>
export default {
    setup() {
    return {
      slider2: 50,

      items: [
       
       
      ],
    };
  },
}
</script>

<style>
.first {
  width: 100%;
  padding: 2rem;
}

.child {
  text-align: center;
  margin-bottom: 1.5rem;
}
.imgHover {
  padding: 0 200px;
}
</style>