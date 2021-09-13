<template>
  <v-app-bar app class="navbar_container" height="150">
    <v-img
      src="../assets/logoneg.png"
      alt="logo"
      max-width="12rem"
      contain
    ></v-img>
    <div class="middle_section">
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
          <v-btn large text color="white" class="profile_button"
            >Mi cuenta</v-btn
          >
          <v-btn large outlined color="#ddd">$0,00</v-btn>
        </div>
      </div>
      <div class="navbar_bottom_section">
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
  }

  .middle_section {
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
  }

  .navbar_top_section {
    width: 100%;
    display: flex;
    justify-content: space-between;
    padding-left: 2rem;
  }

  .search_input_container {
    width: 100%;
    max-width: 40rem;
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

  .navbar_bottom_section {
    width: 100%;
    padding-left: 2rem;
    display: flex;
    justify-content: space-between;
  }

  .navbar_bottom_section > ul {
    width: 80%;
    list-style: none;
    padding: 0;
    display: flex;
    color: whitesmoke;
    justify-content: space-between;
    align-items: center;
    font-size: 1.2rem;
  }
</style>
