<template>
  <v-app>
    <v-app-bar app prominent flat class="navbar_container">
      <v-app-bar-nav-icon />
      <img src="../assets/logoneg.png" class="navbar_logo" />
    </v-app-bar>
  </v-app>
</template>

<script>
  export default {
    name: 'Navbar',

    components: {},

    data: () => ({
      //
    }),
  };
</script>

<style scoped>
  .navbar_container {
    background-image: linear-gradient(#212121, #030303);
    padding: 1rem 2rem;
  }

  .navbar_logo {
    width: 12rem;
    object-fit: contain;
  }
</style>
