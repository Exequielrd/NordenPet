<template>
  <v-app-bar app class="navbar_container" height="130">
    <!-- LOGO -->
    <v-row>
      <v-img
        src="../assets/logoneg.png"
        alt="logo"
        max-width="12rem"
        width="15%"
        height="100%"
      ></v-img>

      <div class="middle_section">
        <div class="navbar_top_section">
          <!-- SEARCH CONTAINER -->
          <div class="search_input_container ">
            <input
              class="search_input"
              type="text"
              placeholder="Buscar prductos..."
            />
            <button class="search_button">Buscar</button>
          </div>

          <div class="d-none d-md-flex">
            <v-btn large text color="white">Mi cuenta</v-btn>
            <v-btn large outlined color="#ddd">$0,00</v-btn>
          </div>
          <v-app-bar-nav-icon
            color="white"
            class="d-md-none"
          ></v-app-bar-nav-icon>
        </div>

        <div class="navbar_bottom_section d-none d-md-flex">
          <ul>
            <li>Ofertas</li>
            <li>Perro</li>
            <li>Gato</li>
            <li>Alimentos Humedos</li>
            <li>Alimentos Terapeuticos</li>
            <li>Accesorios</li>
          </ul>
          <v-btn color="#f0ad4e">Envio Gratis</v-btn>
        </div>
      </div>
    </v-row>
  </v-app-bar>
</template>

<script>
  export default {
    name: 'Navbar',

    components: {},
  };
</script>

<style scoped>
  .navbar_container {
    background-image: linear-gradient(#212121, #030303);
    padding: 0 1rem;
  }

  .middle_section {
    width: 85%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  .navbar_top_section {
    display: flex;
    justify-content: space-between;
    padding-left: 2rem;
  }

  .search_input_container {
    width: 60%;
    max-width: 40rem;
    max-height: 3rem;
    background: whitesmoke;
    border: none;
    border-radius: 0.2rem;
    display: flex;
    justify-content: space-between;
  }

  .search_input {
    width: 100%;
    padding: 0.5rem;
    font-size: 1.1rem;
  }

  .search_input_container :focus {
    outline: none;
  }

  .search_button {
    background: #353535;
    color: whitesmoke;
    font-size: 1rem;
    padding: 0.5rem 1rem;
  }

  .navbar_bottom_section {
    width: 100%;
    padding: 1rem 0 0 2rem;
    display: flex;
    justify-content: space-between;
  }

  .navbar_bottom_section > ul {
    width: 80%;
    list-style: none;
    padding: 0;
    display: flex;
    align-items: center;
    gap: 1rem;
    color: whitesmoke;
    font-size: 1rem;
    max-width: 70rem;
  }
</style>
