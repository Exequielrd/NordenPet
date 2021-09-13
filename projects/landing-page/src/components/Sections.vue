<template>
  <v-sheet color="#85b719">
    <v-container fluid>
      <v-container>
        <v-row class="justify-center">
          <v-card
            v-for="i in 6"
            :key="i"
            width="22rem"
            class="d-flex justify-space-between pa-5 ma-2"
          >
            <v-img
              src="https://nordenpet.com.ar/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/elementor/thumbs/alimento-terapeutico-pab2pfrd0qakung0c1npl03ktm8kiso0lil80cq9s0.png.webp"
              contain
              max-width="30%"
            />
            <v-col class="d-flex flex-column align-center">
              <v-sheet width="80%">
                <v-card-title class="pa-0 text-center title">
                  ALIMENTOS TERAPEUTICOS
                </v-card-title>
              </v-sheet>
              <v-btn width="8rem" depressed color="#f0ad4e">Ver mas</v-btn>
            </v-col>
          </v-card>
        </v-row>
      </v-container>
    </v-container>
  </v-sheet>
</template>

<script>
  export default {
    name: 'Sections',
  };
</script>
