<template>
  <v-parallax src="https://www.alpaymermer.com/upload/urunler/blanco_ibiza/Alpay_Mermer_blanco_ibiza_yeni.jpg" class="products" >
    <v-row class="products align-self-center d-flex">
      <v-col cols="2">
        <div id="products" class="position-relative"></div>
      </v-col>
      <v-col cols="8" class="align-self-center">
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
  </v-parallax>

</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Products",
  data() {
    return{
      products: [
          'Kalibre Makinası',
          'Trimming Ebatlama Makinası',
          'Mozaik Çoklu Kesim Makinası',
          'Bantlı Kafa Kesme Makinası',
          'Kafa Kesme Makinası',
          'Strip Robot ve Hattı',
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
    height: 100vh;
  }
</style>
