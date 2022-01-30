<template>
  <MenuPrincipal />
  <div class="container">
    <CaminoMigas />

    <div class="dos-columnas">
      <ProductoImagen />
      <ProductoDatos />
    </div>
    <div class="dos-columnasB">
      <Formulario />
      <Descripcion />
    </div>
  </div>
  <Pie />
</template>

<script>
import MenuPrincipal from "./components/MenuPrincipal.vue";
import CaminoMigas from "./components/CaminoMigas.vue";
import ProductoImagen from "./components/ProductoImagen.vue";
import ProductoDatos from "./components/ProductoDatos.vue";
import Descripcion from "./components/Descripcion.vue";
import Formulario from "./components/Formulario.vue";
import Pie from "./components/Pie.vue";

export default {
  name: "App",
  components: {
    MenuPrincipal,
    CaminoMigas,
    ProductoImagen,
    ProductoDatos,
    Descripcion,
    Formulario,
    Pie,
  },
};
</script>

<style>
body {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
}

#app {
  font-family: Arial, Helvetica, sans-serif;
}
.container {
  margin: auto;
}

.dos-columnas {
  display: flex;
  flex-wrap: wrap;
}

.dos-columnasB {
  display: flex;
  flex-wrap: wrap;
  background-color: beige;
  padding-bottom: 10rem;
}
</style>
