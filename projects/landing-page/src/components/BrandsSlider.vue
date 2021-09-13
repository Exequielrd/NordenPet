<template>
  <v-sheet color="#85b719">
    <v-container fluid>
      <v-container>
        <v-row>
          <section class="brands_header col-md-3">
            <v-img
              width="5rem"
              class="my-10"
              contain
              src="../assets/footprint.webp"
              alt=""
            />
            <h1 class="ma-5 title">LAS MEJORES MARCAS PARA TUS MASCOTAS</h1>
            <v-btn large color="#85b719" class="white--text my-2"
              >VER TODAS</v-btn
            >
          </section>
          <v-carousel
            cycle
            interval="3000"
            hide-delimiters
            height="18rem"
            class="col-md-9 white my-auto"
          >
            <v-carousel-item v-for="(brand, i) in brands" :key="i">
              <img :src="brand" alt="" contain class="ma-10" height="200" />
            </v-carousel-item>
          </v-carousel>
        </v-row>
      </v-container>
    </v-container>
  </v-sheet>
</template>

<script>
  export default {
    name: 'BrandsSlider',

    data: () => ({
      brands: [
        'https://nordenpet.com.ar/wp-content/uploads/2021/07/vitalcan-balanced.png',
        'https://nordenpet.com.ar/wp-content/uploads/2021/07/Vitalcan-complete.png',
      ],
    }),
  };
</script>

<style scoped>
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
  }
</style>
