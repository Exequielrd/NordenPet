<template>
  <v-app-bar app prominent flat class="navbar_container">
    <v-app-bar-nav-icon />
    <img src="../assets/logoneg.png" class="navbar_logo" />
    <div class="navbar_top_section">
      <div class="search_input_container">
        <input
          class="search_input"
          type="text"
          placeholder="Buscar prductos..."
        />
        <button class="search_button">Buscar</button>
      </div>
      <div>
        <v-btn large text color="white" class="profile_button">Mi cuenta</v-btn>
        <v-btn large outlined color="#ddd">$0,00</v-btn>
      </div>
    </div>

    <div class="navbar_bottom_section">
      <div class="navbar_categories"></div>
    </div>
  </v-app-bar>
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
    width: 15%;
    object-fit: contain;
  }

  .navbar_top_section {
    display: flex;
    justify-content: space-between;
    width: 100%;
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
    background: #353535;
    color: whitesmoke;
    font-size: 1rem;
    padding: 0.5rem 1rem;
  }
</style>
