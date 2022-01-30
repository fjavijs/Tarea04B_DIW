<template>
  <section id="producto-imagen">
    <div class="img-big">
      <img
        v-bind:src="fotos[0]"
        alt="vacuna 1"
        copyright="pv-by Fco Javier Jiménez Soler"
      />
    </div>
    <div class="img-mini">
      <a @click="cambiarFoto(1)"
        ><img
          v-bind:src="fotos[1]"
          alt="vacuna 2"
          copyright="pv-by Fco Javier Jiménez Soler"
      /></a>
      <a @click="cambiarFoto(2)"
        ><img
          v-bind:src="fotos[2]"
          alt="vacuna 3"
          copyright="pv-by Fco Javier Jiménez Soler"
      /></a>
      <a @click="cambiarFoto(3)"
        ><img
          v-bind:src="fotos[3]"
          alt="vacuna 4"
          copyright="pv-by Fco Javier Jiménez Soler"
      /></a>
      <a @click="cambiarFoto(4)"
        ><img
          v-bind:src="fotos[4]"
          alt="vacuna 5"
          copyright="pv-by Fco Javier Jiménez Soler"
      /></a>
    </div>
  </section>
</template>

<script>
export default {
  Name: "ProductoImagen",
  data() {
    return {
      fotos: [
        require("../assets/vacunas/e1.jpg"),
        require("../assets/vacunas/e1.jpg"),
        require("../assets/vacunas/e2.jpg"),
        require("../assets/vacunas/e3.jpg"),
        require("../assets/vacunas/e4.jpg"),
      ],
    };
  },
  methods: {
    cambiarFoto(id) {
      this.fotos[0] = this.fotos[id];
    },
  },
};
</script>

<style scoped>
#producto-imagen {
  padding: 1rem;
  margin: 1rem;
  flex: 0 1 50%;
}
.img-mini {
  display: flex;
  justify-content: space-around;
  margin-top: 1rem;
}
.img-big {
  padding-left: 3rem;
}
.img-mini img {
  width: 100px;
  border: 2px solid #11769e;
}
</style>