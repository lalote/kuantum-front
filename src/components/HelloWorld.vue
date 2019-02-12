<template>
  <v-layout text-xs-center wrap>
    <v-flex>
      <v-flex xs12>
        <v-img :src="require('../assets/logo2.png')" contain class="logo"></v-img>
      </v-flex>
      <v-layout class="contenedor">
        <div class="titulo_principal">
          <h1>ENTRENA INTELIGENTE</h1>
        </div>

        <div class="titulo_principal">
          <h2>CUANTIFICA TU PROGRESO</h2>
        </div>

        <v-flex xs12 class="poligono_arriba"></v-flex>

        <!-- <div class="poligono_arriba"></div> -->
        <!--       <v-flex xs12 class="poligono_arriba" row>
        -->
        <!-- <v-img :src="require('../assets/flecha-roja-arriba.png')"  ></v-img> -->
        <!-- <div class="poligono_arriba"></div> -->
        <!--  </v-flex> -->
        <v-flex xs12 class="imagen_danny">
          <v-img :src="require('../assets/danny-face.png')" class="imagen_danny"></v-img>
        </v-flex>

        <v-flex xs12 class="imagen_fondo">
          <v-img :src="require('../assets/imagen_fondo.png')" class="imagen_fondo"></v-img>
        </v-flex>
        <!-- margin bottom mb-4 -->
        <v-flex xs12 class="poligono_abajo">
          <!-- <v-img :src="require('../assets/flecha-roja-abajo.png')"  ></v-img> -->
          <!-- <div class="poligono_abajo"></div> -->
        
      </v-flex>
      </v-layout>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
  data: () => ({})
};
</script>

<style>
.contenedor {
  margin-top: 10px;
}

.logo {
  float: left;
  padding-left: 100px;
  padding-right: 60px;
  margin-left: 20px;
  height: 104px;
}

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
  z-index: 2;
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
  z-index: 2;
}
.imagen_danny {
  position: absolute;
  top: 28px;
  left: 110px;
  width: 100%;
  height: 1460px;
  z-index: 99999;
}
.titulo_principal {
  width: 100%;
  position: absolute;
  top: 220px;
  z-index: 1000;
}

.titulo_principal h1 {
  text-align: center;
  color: white;
  font-size: 9vw;
  font-family: "Helvetica LT Std", Helvetica-LT-Std-Ultra-Compressed;
  display: block;
  clear: both;
}
.titulo_principal h2 {
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
