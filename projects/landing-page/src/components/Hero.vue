<template>
  <v-main>
    <HeaderCarousel />
    <OffersSlider />
    <BrandsSlider />
    <DogsCategory />
    <CatsCategory />
    <Sections />
  </v-main>
</template>

<script>
  import HeaderCarousel from './HeaderCarousel';
  import OffersSlider from './OffersSlider';
  import BrandsSlider from './BrandsSlider';
  import DogsCategory from './DogsCategory';
  import CatsCategory from './CatsCategory';
  import Sections from './Sections';

  export default {
    name: 'Hero',

    components: {
      HeaderCarousel,
      OffersSlider,
      BrandsSlider,
      DogsCategory,
      CatsCategory,
      Sections,
    },
  };
</script>
