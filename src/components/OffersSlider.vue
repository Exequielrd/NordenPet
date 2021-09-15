<template>
  <v-container class="pt-10 pb-10 max-width">
    <!-- TITLE -->
    <v-row align-content="center" class="pl-10 col-xl-8 ma-auto">
      <v-img max-width="2.5rem" contain src="../assets/footprint.webp" alt="" />
      <h1 class="offers_title">OFERTAS NORDENPET</h1>
    </v-row>

    <!-- Slider -->
    <v-sheet class="mx-auto" max-width="1000">
      <v-slide-group class="mt-10" show-arrows center-active>
        <v-slide-item v-for="i in 5" :key="i">
          <v-card class="ma-4 pa-2" width="200">
            <v-img
              src="https://nordenpet.com.ar/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2019/10/Vitalcan-Balanced-Gato-Control-PH-300x300.jpg.webp"
            />
            <v-card-title
              class="text-center subtitle-2 font-weight-semibold pa-2"
            >
              Vitalcan Balanced Gato Control PH
            </v-card-title>

            <v-card-text class="pa-1">
              <div class="subtitle-1 text-center">
                Desde:
                <b>
                  $1230,00
                </b>
              </div>
            </v-card-text>
            <v-row justify="center" class="pl-6 pr-6 pb-4 pt-2">
              <v-btn color="#f0ad4e" class="white--text" block>
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

  .v-icon {
    box-shadow: 1rem 1rem 5rem black !important;
  }
</style>
