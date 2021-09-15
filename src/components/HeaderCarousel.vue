<template>
  <v-carousel cycle hide-delimiters height="auto">
    <v-carousel-item
      v-for="(slide, i) in slides.desktop"
      :key="i"
      :src="slide"
      contain
    >
    </v-carousel-item>
  </v-carousel>
</template>

<script>
  export default {
    name: 'HeaderCarousel',

    data: () => ({
      slides: {
        mobile: [],
        desktop: [
          'https://nordenpet.com.ar/wp-content/uploads/2021/07/slide-bienvenidos-JUL-2021-Desktop.jpg',
          'https://nordenpet.com.ar/wp-content/uploads/2021/09/Asistente-Nordenpet-Desktop.png',
          'https://nordenpet.com.ar/wp-content/uploads/2021/07/slide-envios-v2-jul-2021-desktop.jpg',
          'https://nordenpet.com.ar/wp-content/uploads/2021/07/slide-eukanuba-AGO-2021-desktop.jpg',
          'https://nordenpet.com.ar/wp-content/uploads/2021/07/slide-promo-royalcanin-JUL-2021-desktop.jpg',
        ],
      },
    }),
  };
</script>
