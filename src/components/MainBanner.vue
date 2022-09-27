<template>
  <div id="main"></div>
  <v-parallax src="https://www.destekkaynak.com/wp-content/uploads/2022/04/s1.jpg" class="main-banner">
    <v-row class="align-center h-100 text-white">
      <v-col class="text-center">
        <h1 class="text-h2 font-weight-thin mb-4">
          OKUMER MAKINE
        </h1>
        <h3 class="subheading">
          Düşün! Tasarla! Üret!
        </h3>
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
   height: 100vh;
 }
</style>
