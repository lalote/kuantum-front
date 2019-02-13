<template>
  <section class="contenedor">
    <v-flex xs12 class="logo">
      <v-img :src="require('../assets/logo2.png')" contain></v-img>
    </v-flex>


      <v-flex xs12 class="poligono_arriba"></v-flex>

      <div class="titulo_principal">
        <h1>ENTRENA INTELIGENTE</h1>
      </div>

      <div class="titulo_principal">
        <h2>CUANTIFICA TU PROGRESO</h2>
      </div>

      <v-flex xs12 class="imagen_danny">
        <v-img :src="require('../assets/danny-face.png')" class="imagen_danny"></v-img>
      </v-flex>
    
    <!-- <div class="poligono_arriba"></div> -->
    <!--       <v-flex xs12 class="poligono_arriba" row>
    -->
    <!-- <v-img :src="require('../assets/flecha-roja-arriba.png')"  ></v-img> -->
    <!-- <div class="poligono_arriba"></div> -->
    <!--  </v-flex> -->
    <v-flex xs12 fill class="imagen_fondo">
      <v-img :src="require('../assets/imagen_fondo.png')" class="imagen_fondo"></v-img>
    </v-flex>
    <!-- margin bottom mb-4 -->
    <v-flex xs12 class="poligono_abajo">
      <!-- <v-img :src="require('../assets/flecha-roja-abajo.png')"  ></v-img> -->
      <!-- <div class="poligono_abajo"></div> -->
    </v-flex>
  </section>
</template>

<script>
export default {
  data: () => ({})
};
</script>

<style>
.contenedor {
  margin-top: 10px;
  position: relative;
  width: 100%;
  height: 100%;
}

.logo {
  position: absolute;
}

.poligono_arriba {
  -webkit-clip-path: polygon(
    37% 12%,
    54% 74%,
    100% 2%,
    100% 37%,
    52% 94%,
    36% 29%,
    0% 91%,
    0% 80%
  );
  clip-path: polygon(
    37% 12%,
    54% 74%,
    100% 2%,
    100% 37%,
    52% 94%,
    36% 29%,
    0% 91%,
    0% 80%
  );
  height: 120px;
  width: 100%;
  background: red;
  position: relative;
  z-index: 2;
  top: 92px;
}
.poligono_abajo {
  -webkit-clip-path: polygon(
    0% 62%,
    46% 3%,
    62% 71%,
    100% 3%,
    100% 12%,
    61% 88%,
    45% 25%,
    0 95%
  );
  clip-path: polygon(
    0% 62%,
    46% 3%,
    62% 71%,
    100% 3%,
    100% 12%,
    61% 88%,
    45% 25%,
    0 95%
  );
  height: 118px;
  background: red;
  position: relative;
  top: -92px;
}
.imagen_fondo {
  -webkit-clip-path: polygon(
    0 15%,
    36% 1%,
    52% 16%,
    100% 3%,
    100% 85%,
    62% 99%,
    47% 84%,
    0% 97%
  );
  clip-path: polygon(
    0 15%,
    36% 1%,
    52% 16%,
    100% 3%,
    100% 85%,
    62% 99%,
    47% 84%,
    0% 97%
  );

  height: 521px;
  z-index: 2;
  width: 100%;
  object-fit: fill;
}
.imagen_danny {
  top : -50px;

  position: relative;
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
