<template>
  <v-main>
    <v-carousel>
      <v-carousel-item v-for="(slide, i) in slides" :key="i" :src="slide">
      </v-carousel-item>
    </v-carousel>
  </v-main>
</template>

<script>
  export default {
    name: 'Hero',

    data: () => ({
      slides: [
        '../assets/slide_1.jpg',
        '../assets/slide_2.png',
        '../assets/slide_3.jpg',
        '../assets/slide_4.jpg',
        '../assets/slide_5.jpg',
      ],
    }),
  };
</script>
