<template>
  <v-card class="overflow-hidden navigation">
    <v-app-bar
        height="50"
        color="white"
    >
      <v-btn plain href="#main">
        <img :src="require('@/assets/logo_1.jpeg')" style="height: 32px">
      </v-btn>
      <v-spacer></v-spacer>
      <v-btn href="#about-us" scroll-target="#about-us" elevate-on-scroll>
        Hakkimizda
      </v-btn>
      <v-btn href="#products">
        Ürünlerimiz
      </v-btn>
      <v-btn href="#contact-us">
        Bize Ulaşın
      </v-btn>
    </v-app-bar>
  </v-card>
</template>

<script>
export default {
  name: "NavigationBar"
}
</script>

<style scoped>
  .navigation {
    z-index: unset !important;
  }
</style>
