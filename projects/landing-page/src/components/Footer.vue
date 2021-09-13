<template>
  <v-container fluid class="footer_container">
    <v-container>
      <!-- Firs Column -->
      <v-row>
        <v-col md="4">
          <v-img src="../assets/logoneg.png" width="15rem" contain />
          <address class="footer_address">
            <strong>Direccion</strong> Av Veles Sarfield 4634, Munro Provincia
            de Buenos Aires <strong>Whatsapp</strong> (011) 15-55-69-3758
            <strong>Telefono</strong> (011) 4509-6793
            <strong>Email</strong> ventas@nordenpet.com.ar
          </address>
        </v-col>

        <!-- Second Column -->
        <v-col md="4">
          <h1 class="footer_title">institucional</h1>
          <ul class="footer_list">
            <li>sobre nordenpet</li>
            <li>zonas de cobertura para envios</li>
            <li>dejanos un mensaje</li>
            <li>novedades</li>
          </ul>
          <h1 class="footer_title mt-10">ofertas semanales por whatsapp</h1>
        </v-col>

        <!-- Third Column -->
        <v-col md="4">
          <h1 class="footer_title">data fiscal</h1>
          <v-img
            src="https://nordenpet.com.ar/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/elementor/thumbs/DATAWEB-pan47cqxftm7euzaqsevzwjr92nv1t2mvmpaatojy8.jpg.webp"
            alt="data fiscal"
            width="5rem"
            contain
          ></v-img>
          <h1 class="footer_title mt-8">segunos en las redes</h1>
        </v-col>
      </v-row>
    </v-container>
  </v-container>
</template>

<script>
  export default {
    name: 'Footer',
  };
</script>

<style scoped>
  .footer_container {
    background-image: linear-gradient(#212121, #030303);
  }

  .footer_address {
    color: gray;
    display: flex;
    flex-direction: column;
  }

  .footer_address > strong {
    padding-top: 0.5rem;
  }

  .footer_title {
    color: #85b719;
    text-transform: uppercase;
    font-size: 1.5rem;
  }

  .footer_list {
    list-style: none;
    padding: 0;
    color: gray;
    text-transform: capitalize;
  }
</style>
