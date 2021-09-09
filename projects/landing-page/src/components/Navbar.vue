<template>
  <v-app>
    <v-app-bar app prominent flat class="navbar_container">
      <v-app-bar-nav-icon />
      <img src="../assets/logoneg.png" class="navbar_logo" />
      <div class="search_input_container">
        <input
          class="search_input"
          type="text"
          placeholder="Buscar prductos..."
        />
        <button class="search_button">Buscar</button>
      </div>
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

  .search_input_container {
    width: 40rem;
    background: whitesmoke;
    border: none;
    border-radius: 0.2rem;
    display: flex;
    justify-content: space-between;
  }

  .search_input_container :focus {
    outline: none;
  }

  .search_input {
    width: 100%;
    padding: 0.5rem;
    font-size: 1.1rem;
  }

  .search_button {
    background: gray;
  }
</style>
