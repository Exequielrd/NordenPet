<template>
  <v-main>
    <v-carousel cycle hide-delimiters height="auto">
      <v-carousel-item
        v-for="(slide, i) in slides"
        :key="i"
        :src="slide.src"
        contain
      >
      </v-carousel-item>
    </v-carousel>
    <v-container class="my-10">
      <div class="offers">
        <h1 class="headline green--text">OFERTAS NORDENPET</h1>
        <v-card
          width="16rem"
          max-width="374"
          class="my-15"
          v-for="index in 6"
          :key="index"
        >
          <v-img
            height="250"
            src="https://nordenpet.com.ar/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2019/10/Vitalcan-Balanced-Gato-Control-PH-300x300.jpg.webp"
            contain
          ></v-img>

          <v-card-title class="text-center"
            >Vitalcan Balanced Gato Control PH</v-card-title
          >

          <v-card-text>
            <div class="headline text-center">
              Desde:
              <span class="font-weight-bold">
                $1230,00
              </span>
            </div>
          </v-card-text>

          <v-card-actions>
            <v-btn color="blue">
              Comprar
            </v-btn>
          </v-card-actions>
        </v-card>
      </div>
    </v-container>
  </v-main>
</template>

<script>
  export default {
    name: 'Hero',

    data: () => ({
      slides: [
        { src: require('../assets/slide_1.jpg') },
        { src: require('../assets/slide_2.png') },
        { src: require('../assets/slide_3.jpg') },
        { src: require('../assets/slide_4.jpg') },
        { src: require('../assets/slide_5.jpg') },
      ],
    }),
  };
</script>

<style scoped>
  .offers {
    max-width: 65rem;
    width: 100%;
    background: red;
    margin: auto;
  }
</style>
