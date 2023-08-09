<template>
  <v-app>
    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
}
</script>

<style>
@media (max-width: 600px) {
  .egg {
    margin-bottom: 1rem;
  }

  .about-content {
    text-align: center;
  }

  .first {
    height: auto;
    padding: 1rem;
  }

  .first .child {
    display: block;
    text-align: center;
    margin-bottom: 1.5rem;
  }
}
</style>
