<template>
  <v-container class="col-xl-8">
    <!-- Image -->
    <v-row class=" mt-15">
      <v-col>
        <ImageCategory
          title="Alimentos para perros"
          image="https://nordenpet.com.ar/wp-content/uploads/2021/07/perros.jpg"
        />
      </v-col>

      <!-- Slider -->
      <v-col cols="12" md="8">
        <v-slide-group show-arrows>
          <v-slide-item v-for="i in 4" :key="i">
            <v-card class="ma-4 pa-2" width="220">
              <v-img
                src="https://nordenpet.com.ar/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2019/10/Vitalcan-Balanced-Gato-Control-PH-300x300.jpg.webp"
              />
              <v-card-title
                class="text-center subtitle-1 font-weight-semibold pt2"
                >Vitalcan Balanced Gato Control PH</v-card-title
              >

              <v-card-text class="pa-0">
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
    </v-row>
  </v-container>
</template>

<script>
  import ImageCategory from './ImageCategory';

  export default {
    name: 'DogsCategory',

    components: {
      ImageCategory,
    },
  };
</script>
