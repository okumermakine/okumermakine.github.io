<template>
  <v-row class="products d-flex bg-brown-lighten-5">
    <v-col cols="2">
      <div id="products" class="position-relative"></div>
    </v-col>
    <v-col cols="8" class="align-self-center ">
      <h1 class="py-10 text-center text-h4">Ürünlerimiz</h1>
      <v-row class="align-content-center">
          <v-col
            cols="4"
            v-for="product in products"
            :key="product[0]">
            <v-card
                elevation="2"
                class="d-flex align-center justify-center text-center card pa-3 bg-brown-lighten-4"
            >
              <h4 class="text-h6 text-grey-darken-2"> {{ product }} </h4>
            </v-card>
          </v-col>
      </v-row>
    </v-col>
  </v-row>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Products",
  data() {
    return{
      products: [
          'Kalibre Makinası',
          'Trimming Ebatlama makinası',
          'Mozaik Çoklu Kesim makinası',
          'Bantlı Kafa Kesme Makinası',
          'Kafa Kesme Makinası',
          'Kenar Kırma ve Eskitme Hattı',
          'Bulnos Makinası',
          'Dekoratif Patlatma Makinası',
          'Mozaik Patlatma Makinası',
          'Otomatik Patlatma Makinası',
          'Mermer Makinaları Revizyonu',
      ],
    };
  },
  methods: {
    rowCount() {
      let counts = this.products.length;
      if (counts % 3 !== 0) {
        return counts / 3 + 1
      }
      return counts / 3
    },
  },
}
</script>

<style scoped>
  .card {
    height: 120px;
  }
  .products {
    height: 105vh;
  }
</style>
