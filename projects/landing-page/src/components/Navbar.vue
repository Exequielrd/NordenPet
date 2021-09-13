<template>
  <v-app-bar app prominent flat class="navbar_container">
    <img src="../assets/logoneg.png" class="navbar_logo" />
    <v-col>
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

      <div class="navbar_categories">
        <ul>
          <li>Ofertas</li>
          <li>
            Perro
            <ul class="subnav">
              <div class="ml-10 mr-10">
                Marca
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
              </div>
              <div class="ml-10 mr-10">
                Marca
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
              </div>
            </ul>
          </li>

          <li>
            Gato
            <ul class="subnav">
              <div class="ml-10 mr-10">
                Marca
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
              </div>
              <div class="ml-10 mr-10">
                Marca
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
              </div>
            </ul>
          </li>
          <li>
            Alimentos Humedos
            <ul class="subnav">
              <div class="ml-10 mr-10">
                Marca
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
              </div>
              <div class="ml-10 mr-10">
                Marca
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
              </div>
            </ul>
          </li>
          <li>
            Alimentos Terapeuticos
            <ul class="subnav">
              <div class="ml-10 mr-10">
                Marca
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
              </div>
              <div class="ml-10 mr-10">
                Marca
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
              </div>
            </ul>
          </li>
          <li>
            Accesorios
            <ul class="subnav">
              <div class="ml-10 mr-10">
                Marca
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
              </div>
              <div class="ml-10 mr-10">
                Marca
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
                <li>Item</li>
              </div>
            </ul>
          </li>
        </ul>
      </div>
    </v-col>
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

  .navbar_categories {
    color: whitesmoke;
    height: 100%;
  }

  .navbar_categories > ul {
    list-style: none;
    padding: 0;
    display: flex;
    justify-content: space-around;
    font-size: 1rem;
  }

  .navbar_categories ul li:hover > ul {
    display: flex;
  }

  .subnav {
    list-style: none;
    padding: 0;
    display: none;
    background: whitesmoke;
    color: #333;
    padding: 2rem;
    font-weight: 600;
    font-size: 1.2rem;
    border-top: 5px solid #85b719;
    position: absolute;
    transform: translateX(-10rem);
  }

  .subnav li {
    font-weight: 400;
    font-size: 1rem;
    margin: 1rem 0;
  }
</style>
