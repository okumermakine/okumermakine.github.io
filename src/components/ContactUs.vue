<template>
<v-row class="contact-us d-flex">
  <v-col cols="3">
    <div id="contact-us" class="position-relative"></div>
  </v-col>
  <v-col cols="6" class="align-self-center ">
    <h1 class="mb-8 text-center">Bize Ulaşın</h1>
    <p class="text-center mb-3">
          Okumer Makine Endüstri Sanayi ve Ticaret Limited Şirketi
    </p>
    <p class="text-center mb-3">
          okumermakine@gmail.com
    </p>
    <p class="text-center mb-3">
          info@okumer.com
    </p>
    <p class="text-center mb-3">
          +(90) 541 455 87 74
    </p>
    <p class="text-center mb-3">
          Eskihisar Mh. 8021.Sk. No:8 Hurdacılar Sitesi/Merkezefendi/Denizli <br>
    </p>
    <div class="d-flex justify-space-around mt-5">
      <v-btn icon x-large>
        <v-icon icon>mdi-facebook</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon icon>mdi-twitter</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon icon>mdi-instagram</v-icon>
      </v-btn>
    </div>
  </v-col>
</v-row>
</template>

<script>
export default {
  name: "ContactUs"
}
</script>

<style scoped>
  .contact-us {
    height: 105vh;
  }
</style>
