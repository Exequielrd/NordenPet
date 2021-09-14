<template>
  <v-sheet color="#85b719">
    <v-container fluid class="pt-15 pb-15 pl-5 pr-5">
      <v-row class="justify-center justify-md-start">
        <v-col v-for="i in 6" :key="i" cols="12" md="4">
          <v-card width="100%" class="d-flex justify-space-between pa-4">
            <v-row>
              <v-col cols="12" sm="4" align-self="center">
                <v-img
                  src="https://nordenpet.com.ar/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/elementor/thumbs/alimento-terapeutico-pab2pfrd0qakung0c1npl03ktm8kiso0lil80cq9s0.png.webp"
                  contain
                  width="50%"
                  class="ma-auto"
                />
              </v-col>
              <v-col cols="12" sm="8" class="d-flex flex-column align-center">
                <v-card-title class="pa-0 text-center title gray--text">
                  ALIMENTOS <br />
                  TERAPEUTICOS
                </v-card-title>
                <v-btn width="8rem" depressed color="#f0ad4e" class="mt-5"
                  >Ver mas</v-btn
                >
              </v-col>
            </v-row>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-sheet>
</template>

<script>
  export default {
    name: 'Sections',
  };
</script>
