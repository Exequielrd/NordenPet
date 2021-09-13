<template>
  <v-container>
    <v-row>
      <v-slide-group class="mt-10 col-md-8" show-arrows>
        <v-slide-item v-for="i in 6" :key="i">
          <v-card class="ma-4 pa-2" width="220">
            <v-img
              src="https://nordenpet.com.ar/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2019/10/Vitalcan-Balanced-Gato-Control-PH-300x300.jpg.webp"
            />
            <v-card-title class="text-center subtitle-1 font-weight-bold"
              >Vitalcan Balanced Gato Control PH</v-card-title
            >

            <v-card-text>
              <div class="title text-center">
                Desde:
                <b>
                  $1230,00
                </b>
              </div>
            </v-card-text>
            <v-row justify="center" class="pa-4">
              <v-btn color="#f0ad4e" block>
                Comprar
              </v-btn>
            </v-row>
          </v-card>
        </v-slide-item>
      </v-slide-group>
      <ImageCategory
        title="Alimentos para gatos"
        image="https://nordenpet.com.ar/wp-content/uploads/2021/07/gatos.jpg"
      />
    </v-row>
    <aside class="subscribe_section">
      <h1>
        Suscribite a nuestro <strong>newsletter</strong> para recibir
        <strong>ofertas y novedades</strong>
      </h1>
      <form class="subscribe_form">
        <div class="input_container">
          <input type="email" placeholder="Email" />
          <v-btn dark depressed>Enviar</v-btn>
        </div>
      </form>
    </aside>
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
    margin: 2rem 4rem;
    text-align: center;
    text-transform: uppercase;
    font-weight: 200;
  }

  .subscribe_form {
    background-color: #85b719;
    width: 50%;
    min-height: 100%;
    display: grid;
    place-items: center;
    padding: 0 3rem;
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
</style>
