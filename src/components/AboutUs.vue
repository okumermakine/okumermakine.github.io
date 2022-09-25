<template>
  <v-row class="d-flex bg-blue-grey-lighten-5 about-us">
    <v-col
        cols="2"
    >
      <div id="about-us" class="position-relative"></div>
    </v-col>
    <v-col
      cols="8"
      class="align-content-center align-self-center"
    >
      <h1 class="mb-10 text-center text-h4">Hakkımızda</h1>
      <v-sheet
          :elevation="6"
          class="mx-auto mt-5 text-center pa-3 text-h6 text-grey-darken-1"
      >
        2021 yılında Denizli'de kurulan OKUMER Makine; yüksek hız ve kalite ile üretime yüksek katma değer getiren mermer makinalarını Türkiye'de başarıyla imal etmektedir.
        Teknolojik donanım ve yetkili servis ağı ile sektöre fayda sağlamak; Çözüm ortaklarına katma değer yaratmak için belirlediği bu yolda başarıyla ilerlemektedir.
        Ayrıca işletmelerin üretim verimliliğini en üst düzeye çıkarmaya ve Türk imalat sanayisinin gücüne güç katmaya devam etmektedir.
        Her müşterimize sunduğumuz hizmet kalitesi, bir sonraki müşterimizin de gücüdür.
        Tüm süreçten sorumlu olan OKUMER Makine, her zaman müşterinin başarısını ön planda tutar.
        OKUMER Makina, iş değerleriyle dolu, çevik, açık, dürüst, paylaşımcı ve cesur; Günümüz insan odaklı kurum kültürü ve davranışı ile hareket ederek, gücünü, empatisini ve duyarlılığını yaptığı her işe katarak ilerlemektedir.
      </v-sheet>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: "AboutUs",
  data: () => ({
    elevations: [6, 12, 18],
  }),
}

</script>

<style scoped>
  .about-us{
    height: 105vh;
  }
</style>
