<template>
  <div id="main"></div>
  <v-parallax src="https://cdn.vuetifyjs.com/images/backgrounds/vbanner.jpg" class="main-banner">
    <v-row class="align-center h-100 text-white">
      <v-col class="text-center">
        <h1 class="text-h3 font-weight-thin mb-4">
          OkumerMakine
        </h1>
        <h4 class="subheading">
          Düşün! Tasarla! Üret!
        </h4>
      </v-col>
    </v-row>
  </v-parallax>
</template>

<script>
export default {
  name: "MainBanner"
}
</script>

<style scoped>
 .main-banner{
   height: 105vh;
 }
</style>
