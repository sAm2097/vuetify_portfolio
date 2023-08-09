<template>
  <v-col cols="12" class="mt-16" id="about">
    <v-row>
      <v-col cols="12" sm="6">
        <div class="egg" :style="{ backgroundColor: eggColor }">
          <v-img src="005.png" max-height="320" max-width="350"></v-img>
        </div>
      </v-col>
      <v-col cols="12" sm="6">
        <div class="about-content">
          <h5 class="mt-16">About me</h5>
          <div style="width: 120px">
            <v-slider v-model="slider2" :color="sliderColor"></v-slider>
          </div>
          <h4 class="mt-n4">I am a Web Developer</h4>
          <h4>And Creative Web Designer</h4>
          <p :style="{ color: textColor }">
            Experienced software developer with a solid academic background
            with Masters in Computer Science. Expertise in frontend
            technologies such as JavaScript, TypeScript, HTML, CSS, Vue.js,
            and so on, as well as backend technologies such as Nuxt.js,
            Node.js, Python, Java. Experienced in software development, user
            interface design (Figma), and problem-solving. Shows expertise
            in developing innovative solutions, improving user experience,
            and collaborating effectively in interdisciplinary teams.
            Committed to continuous learning and providing high-quality
            software solutions.
          </p>
          <v-btn tile dark color="yellow" class="mt-4" @click="toResume">
            View Resume
          </v-btn>
        </div>
      </v-col>
    </v-row>
  </v-col>
</template>

<script>
export default {
  data() {
    return {
      slider2: 50,
      eggColor: 'yellow',
    };
  },
  computed: {
    textColor() {
      return this.slider2 === 50 ? 'grey' : this.getRandomColor();
    },
    sliderColor() {
      return this.slider2 === 50 ? 'yellow' : this.getRandomColor();
    },
  },
  methods: {
    getRandomColor() {
      const r = Math.floor(Math.random() * 256);
      const g = Math.floor(Math.random() * 256);
      const b = Math.floor(Math.random() * 256);
      return `rgb(${r},${g},${b})`;
    },
    updateEggColor() {
      if (this.slider2 === 50) {
        this.eggColor = 'yellow';
      } else {
        this.eggColor = this.getRandomColor();
      }
    },
    toResume(){
      this.$router.push({name:'cv'})
    }
  },
  watch: {
    slider2() {
      this.$nextTick(() => {
        this.updateEggColor();
      });
    },
  },
  created() {
    this.$nextTick(() => {
      this.updateEggColor();
    });
  },
};
</script>

<style scoped>
.egg {
  margin: 0 auto 1rem;
  width: 100%;
  max-width: 350px;
  height: auto;
  border: 2px solid;
  background-color: yellow;
  border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
  overflow: hidden;
}

.egg .v-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
  background-color: yellow;
}

</style>
