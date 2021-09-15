<template>
  <v-container class="col-xl-8">
    <!-- Slider -->
    <v-row>
      <v-col md="8" cols="12">
        <v-slide-group class="mt-10" show-arrows>
          <v-slide-item v-for="i in 4" :key="i">
            <v-card class="ma-4 pa-2" width="220">
              <v-img
                src="https://nordenpet.com.ar/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2019/10/Vitalcan-Balanced-Gato-Control-PH-300x300.jpg.webp"
              />
              <v-card-title
                class="text-center subtitle-1 font-weight-semibold pb-0"
                >Vitalcan Balanced Gato Control PH</v-card-title
              >

              <v-card-text class="pa-1">
                <div class="title text-center">
                  Desde:
                  <b>
                    $1230,00
                  </b>
                </div>
              </v-card-text>
              <v-row justify="center" class="pa-4">
                <v-btn color="#f0ad4e" block class="white--text">
                  Comprar
                </v-btn>
              </v-row>
            </v-card>
          </v-slide-item>
        </v-slide-group>
      </v-col>

      <!-- Image -->
      <v-col cols="4">
        <ImageCategory
          title="Alimentos para gatos"
          image="https://nordenpet.com.ar/wp-content/uploads/2021/07/gatos.jpg"
        />
      </v-col>
    </v-row>

    <!-- Subscribe section -->
    <v-row class=" mt-15 mb-15" tag="aside" align-content="center">
      <v-col class="subscribe_section" cols="12" sm="6">
        <h1>
          Suscribite a nuestro <strong>newsletter</strong> para recibir
          <strong>ofertas y novedades</strong>
        </h1>
      </v-col>
      <v-col class="subscribe_form" cols="12" sm="6">
        <form>
          <div class="input_container">
            <input type="email" placeholder="Email" />
            <v-btn dark depressed>Enviar</v-btn>
          </div>
        </form>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  import ImageCategory from './ImageCategory';
  export default {
    name: 'CatsCategory',

    components: {
      ImageCategory,
    },
  };
</script>

<style scoped>
  .subscribe_section {
    color: whitesmoke;
    display: flex;
    background-image: linear-gradient(#212121, #030303);
  }

  .subscribe_section > h1 {
    text-align: center;
    text-transform: uppercase;
    font-weight: 200;
    font-size: 1.3rem;
  }

  .subscribe_form {
    background-color: #85b719;
    width: 50%;
    min-height: 100%;
    display: grid;
    place-items: center;
  }

  .input_container {
    width: 100%;
    display: flex;
    align-items: center;
    background-color: whitesmoke;
    border-radius: 0.2rem;
  }

  .input_container > input {
    width: 100%;
    min-height: 100%;
    outline: none;
  }

  @media (max-width: 768px) {
    .subscribe_form {
      width: 100%;
      min-height: 5rem;
    }
  }
</style>
