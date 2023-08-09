<template>
  <div class="head">
    <v-row>
      <v-col cols="5">
        <div style="position: relative" class="mt-16">
          <h1 class="text-grey">Hello, & Welcome</h1>
          <h1 class="text-white">I'm Sumanth Anugandula</h1>
          <span class="text-grey">Frontend Developer & Web Designer</span>
          <br />
          <v-btn
            tile
            dark
            class="text-blue mt-11"
            variant="outlined"
            @click="scroll('contact')"
          >
            Contact me
          </v-btn>
        </div>
      </v-col>
      <v-col cols="2">
        <div
          style="
            position: absolute;
            z-index: 9999;
            bottom: 0;
            margin-left: auto;
            margin-right: auto;
            left: 0;
            right: 0;
            text-align: center;
          "
        >
          <v-icon>fas fa-angle-double-down</v-icon>
        </div>
      </v-col>
      <v-col cols="5">
        <div style="position: relative; z-index: 9999" class="mt-16">
          <v-img
            src="7.jpg"
            max-height="290"
            max-width="350"
            style="transform: scale(1.1)"
          >
          </v-img>
        </div>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  methods: {
    scroll(refName) {
      const element = document.getElementById(refName);
      element.scrollIntoView({ behavior: "smooth" });
    },
  },
};
</script>

<style>
.head {
  position: relative;
  text-align: center;
  padding: 12px;
  margin-bottom: 6px;
  margin-top: 6px;
  height: 400px;
  width: 100%;
  color: white;
  z-index: 1;
}

.head:before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 50%;
  background: black;
  transform: skew(0deg, 6deg);
}

.head:after {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  height: 100%;
  width: 50%;
  background: black;
  transform: skew(0deg, -6deg);
}
</style>
