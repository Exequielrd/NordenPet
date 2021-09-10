<template>
  <v-app>
    <Navbar />
    <Hero />
  </v-app>
</template>

<script>
  import Navbar from './components/Navbar';
  import Hero from './components/Hero';

  export default {
    name: 'App',

    components: {
      Navbar,
      Hero,
    },

    data: () => ({
      //
    }),
  };
</script>
