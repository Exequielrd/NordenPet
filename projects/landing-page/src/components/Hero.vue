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
    <v-container class="my-10 pl-0">
      <div>
        <div class="title_container">
          <v-img
            max-width="2.5rem"
            contain
            src="../assets/footprint.webp"
            alt=""
          />
          <h1 class="offers_title">OFERTAS NORDENPET</h1>
        </div>
        <div class="offers">
          <v-card
            width="14rem"
            max-width="374"
            class="my-15 mx-4 pa-2"
            v-for="index in 6"
            :key="index"
          >
            <v-img
              height="200"
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
              <v-btn color="#f0ad4e" block>
                Comprar
              </v-btn>
            </v-card-actions>
          </v-card>
        </div>
      </div>
    </v-container>

    <v-container class="brands_slider">
      <section class="brands_header">
        <v-img
          width="5rem"
          class="my-10"
          contain
          src="../assets/footprint.webp"
          alt=""
        />
        <h1 class="ma-5 title">LAS MEJORES MARCAS PARA TUS MASCOTAS</h1>
        <v-btn large color="#85b719" class="white--text my-2">VER TODAS</v-btn>
      </section>
      <BrandsSlider />
    </v-container>
  </v-main>
</template>

<script>
  import BrandsSlider from './BrandsSlider';

  export default {
    name: 'Hero',

    components: {
      BrandsSlider,
    },

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
    width: 100%;
    margin: auto;
    display: flex;
    justify-content: space-between;
    overflow: scroll;
  }

  .title_container {
    display: flex;
    align-items: center;
    margin-bottom: 2rem;
  }

  .offers_title {
    color: #85b719;
    font-weight: 400;
    border-bottom: 2px solid #85b719;
    width: 100%;
    margin-left: 1rem;
  }

  .brands_slider {
    background: #85b719;
    position: relative;
  }

  .brands_header {
    width: 18rem;
    padding: 0 2rem;
    background-image: linear-gradient(#212121, #030303);
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    color: whitesmoke;
    box-shadow: 1rem 0 2rem rgba(26, 26, 26, 0.692);
    position: absolute;
    z-index: 5;
  }
</style>
