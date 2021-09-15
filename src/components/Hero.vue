<template>
  <v-main>
    <HeaderCarousel />
    <OffersSlider />
    <BrandsSlider />
    <DogsCategory />
    <CatsCategory />
    <Sections />
    <Info />
  </v-main>
</template>

<script>
  import HeaderCarousel from './HeaderCarousel';
  import OffersSlider from './OffersSlider';
  import BrandsSlider from './BrandsSlider';
  import DogsCategory from './DogsCategory';
  import CatsCategory from './CatsCategory';
  import Sections from './Sections';
  import Info from './Info';

  export default {
    name: 'Hero',

    components: {
      HeaderCarousel,
      OffersSlider,
      BrandsSlider,
      DogsCategory,
      CatsCategory,
      Sections,
      Info,
    },
  };
</script>
