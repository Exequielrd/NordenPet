<template>
  <v-sheet class="mx-auto" elevation="8">
    <v-carousel cycle hide-delimiters height="20rem">
      <v-slide-group class="pa-4" show-arrows>
        <v-slide-item v-for="(brand, i) in brands" :key="i">
          <img :src="brand" alt="" contain class="ma-10" height="200" />
        </v-slide-item>
      </v-slide-group>
    </v-carousel>
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
