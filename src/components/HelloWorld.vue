<template>
  <v-layout wrap fluid class="text-xs-center">
    <v-flex xs12 sm12 offset-xs4 offset-sm1 offset-md1 offset-lg1>
      <v-img :src="require('../assets/logo2-ext.png')" class="logo"></v-img>
    </v-flex>

    <v-flex xs12>
      <v-img :src="require('../assets/web-encabezado-2.png')" class="imagen_danny"></v-img>
    </v-flex>
    <v-flex xs12 class="contenido">
      <v-flex xs12>
        <v-layout
          row
          wrap
          style="padding:30px"
          color="transparent"
          justify-start
          v-bind:style="getLandingSeccion_1_BGColor"
        >
          

          <v-layout wrap>
            <transition name="fade">
              <v-flex xs12 sm4 style="padding:20px">
                <v-card-title class="text-xs-center">
                  <v-layout align-center column justify-center>                    
                    <v-icon x-large color="white" style="font-size:100px;">fa-user-circle</v-icon>
                    <h2 color="white">Entrenamiento Personalizado</h2>
                  </v-layout>
                </v-card-title>

                <v-card>
                  <v-layout style="padding:20px">
                    <p></p>
                  </v-layout>
                </v-card>
              </v-flex>
            </transition>

            <transition name="fade">
              <v-flex xs12 sm4 style="padding:20px">
                <v-card-title class="text-xs-center">
                  <v-layout align-center justify-center>
                    <v-icon x-large color="white" style="font-size:100px;">favorite_border</v-icon>
                  </v-layout>
                </v-card-title>
                <v-layout style="padding:20px">
                  <p>Progressively build 2.0 manufactured products before go forward partnerships. Rapidiously matrix go forward initiatives without cross-platform potentialities. Enthusiastically matrix mission-critical paradigms whereas high-quality value.</p>
                </v-layout>
              </v-flex>
            </transition>
            <transition name="fade">
              <v-flex xs12 sm4 style="padding:20px">
                <v-card-title class="text-xs-center">
                  <v-layout align-center justify-center>
                    <v-icon x-large color="white" style="font-size:100px;">fa-dumbbell</v-icon>
                  </v-layout>
                </v-card-title>
                <v-layout style="padding:20px">
                  <p>Progressively build 2.0 manufactured products before go forward partnerships. Rapidiously matrix go forward initiatives without cross-platform potentialities. Enthusiastically matrix mission-critical paradigms whereas high-quality value.</p>
                </v-layout>
              </v-flex>
            </transition>
          </v-layout>
        </v-layout>
      </v-flex>
    </v-flex>
  </v-layout>
</template>

<script>
import { mapGetters } from "vuex";
export default {
  data() {
    return {
      seccion1: false,
      seccion2: false,
      seccion3: false,
      seccion4: false,
      emailErrors: [],
      email: "",
      loading: false
    };
  },
  components: {
    name: "Home"
  },
  methods: {
    getPosts() {},
    submit() {}
  },
  computed: {
    ...mapGetters({
      getLandingSeccion_1_BGColor: "getLandingSeccion_1_BGColor",
      getLandingSeccion_2_BGColor: "getLandingSeccion_2_BGColor",
      getLandingSeccion_3_BGColor: "getLandingSeccion_3_BGColor",
      getLandingSeccion_4_BGColor: "getLandingSeccion_4_BGColor",
      getLandingSeccion_5_BGColor: "getLandingSeccion_5_BGColor"
    })
  }
};
</script>

<style>
.contenido {
  height: 100%;
  background-color: #181819;
}

.logo {
  width: 202px;
  height: 104px;
  top: 10px;
}

.imagen_danny {
  top: 20px;
  background-color: #1f1f1f;
  width: 100%;
  height: 100%;
  clip-path: polygon(
    0 18%,
    66% 6%,
    68% 0%,
    100% 0%,
    100% 100%,
    62% 100%,
    27% 100%,
    0% 100%
  );
}
</style>
