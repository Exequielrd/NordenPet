<template>
  <v-container class="pa-15">
    <v-row align-content="center">
      <v-img max-width="2.5rem" contain src="../assets/footprint.webp" alt="" />
      <h1 class="offers_title">OFERTAS NORDENPET</h1>
    </v-row>
    <v-sheet class="mx-auto">
      <v-slide-group class="mt-10" show-arrows>
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
    </v-sheet>
  </v-container>
</template>

<script>
  export default {
    name: 'OffersSlider',

    data: () => ({}),
  };
</script>

<style scoped>
  .offers_title {
    color: #85b719;
    font-size: 1.7rem;
    font-weight: 400;
    border-bottom: 2px solid #85b719;
    width: 90%;
    margin-left: 1rem;
  }
</style>
