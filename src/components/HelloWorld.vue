<template>
  <v-layout text-xs-center wrap style="height:100%;position:relative;">
    <v-flex>
    <v-flex xs12>
      <v-img :src="require('../assets/logo2.png')" contain height="104" ></v-img>
    </v-flex>

    <v-flex xs12 class="poligono_arriba"></v-flex>

    <!-- <div class="poligono_arriba"></div> -->
    <!--       <v-flex xs12 class="poligono_arriba" row>
    -->
    <!-- <v-img :src="require('../assets/flecha-roja-arriba.png')"  ></v-img> -->
    <!-- <div class="poligono_arriba"></div> -->
    <!--  </v-flex> -->
    <v-flex xs12 class="imagen_fondo">
      <v-img :src="require('../assets/imagen_fondo.png')" class="imagen_fondo"></v-img>
    </v-flex>
    <!-- margin bottom mb-4 -->
    <v-flex xs12 class="poligono_abajo">
      <!-- <v-img :src="require('../assets/flecha-roja-abajo.png')"  ></v-img> -->
      <!-- <div class="poligono_abajo"></div> -->
    </v-flex>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
  data: () => ({})
};
</script>

<style>
.poligono_arriba {
  -webkit-clip-path: polygon(
    0% 22%,
    0% 23%,
    36% 13%,
    52% 24%,
    100% 15%,
    100% 9%,
    54% 21%,
    37% 11%
  );
  clip-path: polygon(
    0% 22%,
    0% 23%,
    36% 13%,
    52% 24%,
    100% 15%,
    100% 9%,
    54% 21%,
    37% 11%
  );
  height: 720px;
  background: red;
  position: relative;
}
.imagen_fondo {
/*   -webkit-clip-path: polygon(
    0 23%,
    36% 13%,
    52% 24%,
    100% 14%,
    100% 74%,
    62% 85%,
    47% 74%,
    0 83%
  ); */
  clip-path: polygon(
    0 23%,
    36% 13%,
    52% 24%,
    100% 14%,
    100% 74%,
    62% 85%,
    47% 74%,
    0 83%
  );

  position: absolute;
  top: 52px;
  width: 100%;
  height: 720px;
  z-index: 99999;
}
.poligono_abajo {
  -webkit-clip-path: polygon(
    0 88%,
    45% 77%,
    61% 88%,
    100% 75%,
    100% 74%,
    63% 84%,
    47% 73%
  );
  clip-path: polygon(
    0 88%,
    45% 77%,
    61% 88%,
    100% 75%,
    100% 74%,
    63% 84%,
    47% 73%
  );
  position: absolute;
  height: 720px;
    width: 100%;
  background: red;
  top: 63px;
}

.triangulo_blanco_abajo_izquierda {
  -webkit-clip-path: polygon(55% 65%, 0 76%, 0 80%);
  clip-path: polygon(55% 65%, 0 76%, 0 80%);
  background: white;
}
.triangulo_blanco_arriba_izquierda {
  -webkit-clip-path: polygon(38% 27%, 0 35%, 0 38%);
  clip-path: polygon(38% 27%, 0 35%, 0 38%);
  background: white;
}

.triangulo_rojo_abajo_derecha {
  -webkit-clip-path: polygon(100% 68%, 74% 77%, 100% 70%);
  clip-path: polygon(100% 68%, 74% 77%, 100% 70%);
  background: red;
}

.triangulo_rojo_arriba_derecha {
  -webkit-clip-path: polygon(100% 68%, 74% 77%, 100% 70%);
  clip-path: polygon(100% 68%, 74% 77%, 100% 70%);
  background: red;
}
</style>
