<template>
  <v-sheet color="#85b719">
    <v-container fluid>
      <v-row class="max_whidt ">
        <v-col cols="12" md="4">
          <section class="brands_header pt-10 pb-10">
            <v-img width="5rem" contain src="../assets/footprint.webp" alt="" />
            <h1 class="ma-5 title">LAS MEJORES MARCAS PARA TUS MASCOTAS</h1>
            <v-btn large color="#85b719" class="white--text my-2"
              >VER TODAS</v-btn
            >
          </section>
        </v-col>

        <v-col
          cols="12"
          md="8"
          align-self="center"
          class="d-flex brands_container white"
        >
          <v-img
            v-for="(brand, i) in brands"
            :key="i"
            :src="brand"
            width="12rem"
            contain
            class="mr-10"
          />
        </v-col>
      </v-row>
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
        'https://nordenpet.com.ar/wp-content/uploads/2021/07/Vitalcan-complete.png',
        'https://nordenpet.com.ar/wp-content/uploads/2021/07/Vitalcan-complete.png',
        'https://nordenpet.com.ar/wp-content/uploads/2021/07/Vitalcan-complete.png',
      ],
    }),
  };
</script>

<style scoped>
  .brands_header {
    width: 100%;
    padding: 0 2rem;
    background-image: linear-gradient(#212121, #030303);
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    color: whitesmoke;
    box-shadow: 1rem 0 2rem rgba(26, 26, 26, 0.692);
  }

  .brands_container {
    overflow: scroll;
    scrollbar-width: 0;
  }

  ::-webkit-scrollbar {
    display: none;
  }
</style>
