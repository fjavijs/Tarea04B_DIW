<template>
  <section id="producto-datos">
    <div class="unidades">
      <h1>100 Viales SarCovid-2</h1>
      <h2>330€<span class="iva"> sin IVA: 300€</span></h2>
      <div class="wrapper">
        <button
          class="btn"
          @click="cambiarContador('-1')"
          type="button"
          name="button"
        >
          -
        </button>
        <input class="cantidad" type="text" name="name" :value="contador" />
        <button
          class="btn"
          @click="cambiarContador('1')"
          type="button"
          name="button"
        >
          +
        </button>
      </div>
      <br />
      <button class="boton">
        <span class="material-icons">shopping_cart</span> AÑADIR CARRITO
      </button>
      <h2>Descripción</h2>
      <p>
        Vacuna de ARN mensajero (ARNm). Este tipo de vacuna usa ARNm
        genéticamente modificado para brindarle a tus células instrucciones
        sobre cómo producir la proteína de la espícula que se encuentra en la
        superficie del virus de la COVID-19. Después de la vacunación, tus
        células inmunitarias comienzan a producir las partes de la proteína de
        la espícula y a ubicarlas en la superficie de las células. Esto hace que
        el organismo produzca anticuerpos. Si más tarde te infectas con el virus
        de la COVID-19, estos anticuerpos combatirán el virus. Después de
        entregar las instrucciones, el ARNm se divide inmediatamente. Nunca
        ingresa al núcleo de las células, donde se almacena tu ADN. Tanto la
        vacuna contra la COVID-19 de Pfizer-BioNTech como la de Moderna utilizan
        ARNm.
      </p>
    </div>
  </section>
</template>

<script>
export default {
  Name: "ProductoDatos",
  data() {
    return {
      contador: 1,
    };
  },
  methods: {
    cambiarContador(num) {
      this.contador += +num;
      if (!isNaN(this.contador) && this.contador < 0) {
        this.contador = 0;
      }
    },
  },
};
</script>

<style scoped>
#producto-datos {
  flex: 1 1 18rem;
}
h1 {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 2.5rem;
}
h2 {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 1.7rem;
  color: #11769e;
}
span.iva {
  font-size: 1rem;
  font-family: Arial, Helvetica, sans-serif;
  font-weight: normal;
  color: #282828;
}
.wrapper {
  height: 2rem;
  display: flex;
}

.cantidad {
  border: none;
  text-align: center;
  width: 2rem;
  font-size: 1.2rem;
  border: 1px solid #d8d8d8;
}
.unidades {
  padding-top: 5rem;
  padding-left: 4rem;
}
.btn {
  border: 1px solid #d8d8d8;
  width: 2rem;
}
.boton {
  background-color: #11769e;
  font-size: 0.9rem;
  font-weight: 700;
  color: white;
  padding: 0.7rem 1rem;
  cursor: pointer;
  border-radius: 25px;
  border: none;
}
p {
  margin-top: 2rem;
  margin-right: 3rem;
}
</style>