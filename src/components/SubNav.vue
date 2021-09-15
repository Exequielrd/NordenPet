<template>
  <div class="navbar_bottom_section d-none d-md-flex">
    <ul>
      <li>
        Ofertas
      </li>
      <li>
        Perro
        <ul class="subnav">
          Royal Canin
          <li>item</li>
          <li>item</li>
          <li>item</li>
          <li>item</li>
          <li>item</li>
        </ul>
      </li>
      <li>
        Gato
        <ul class="subnav">
          Royal Canin
          <li>item</li>
          <li>item</li>
          <li>item</li>
          <li>item</li>
          <li>item</li>
        </ul>
      </li>
      <li>
        Alimentos Humedos
        <ul class="subnav">
          Royal Canin
          <li>item</li>
          <li>item</li>
          <li>item</li>
          <li>item</li>
          <li>item</li>
        </ul>
      </li>
      <li>
        Alimentos Terapeuticos
        <ul class="subnav">
          Royal Canin
          <li>item</li>
          <li>item</li>
          <li>item</li>
          <li>item</li>
          <li>item</li>
        </ul>
      </li>
      <li>
        Accesorios
      </li>
    </ul>

    <v-btn color="#f0ad4e" class="white--text">Envio Gratis</v-btn>
  </div>
</template>

<script>
  export default {
    name: 'SubNav',
  };
</script>

<style scoped>
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

  .navbar_bottom_section li {
    cursor: pointer;
    position: relative;
  }

  .subnav {
    min-width: 10rem;
    display: none;
    list-style: none;
    position: absolute;
    background: whitesmoke;
    color: #222;
    padding: 1rem 2rem;
    margin: 0;
    font-weight: 600;
    font-size: 0.9rem;
    border-top: 5px solid #85b719;
  }

  .subnav li {
    font-weight: 400;
    font-size: 0.8rem;
    margin-top: 0.5rem;
  }

  .navbar_bottom_section li:hover > .subnav {
    display: flex;
    flex-direction: column;
  }
</style>
