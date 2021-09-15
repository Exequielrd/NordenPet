<template>
  <v-app>
    <Navbar />
    <Hero />
    <Footer />
  </v-app>
</template>

<script>
  import Navbar from './components/Navbar';
  import Hero from './components/Hero';
  import Footer from './components/Footer';

  export default {
    name: 'App',

    components: {
      Navbar,
      Hero,
      Footer,
    },

    data: () => ({
      //
    }),
  };
</script>

<style>
  .max_whidt {
    max-width: 1440px !important;
    margin: auto;
  }
</style>
