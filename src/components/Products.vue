<template>
  <v-row>
    <v-col cols="2"/>
    <v-col cols="8">
      <h2 class="py-10">Ürünlerimiz</h2>
      <v-row class="align-content-center">
          <v-col
            cols="4"
            v-for="product in products"
            :key="product[0]">
            <v-card
                elevation="2"
                class="text-center card pa-3"
            >
              <h3> {{ product }} </h3>
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
    height: 75px;
    width: 240px;
  }
</style>
