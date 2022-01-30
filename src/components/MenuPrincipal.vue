<template>
  <section id="menu">
    <div class="container">
      <img src="../assets/logo.png" alt="Logotipo" />
    </div>
    <ul>
      <li><a href="#">INICIO</a></li>
      <li><a href="#">ANTIVIRALES</a></li>
      <li><a href="#">ANTIBIOTICOS</a></li>
      <li><a href="#">COVID</a></li>
      <li><a href="#">PROTECCION PERSONAL</a></li>
    </ul>
    <div id="buscador">
      <form @submit.prevent="handleEnviar">
        <input type="text" placeholder="Buscar productos ..." />
        <button class="boton">Buscar</button>
      </form>
    </div>
  </section>
</template>

<script>
export default {
  name: "MenuPrincipal",
  methods: {
    handleSutmit() {
      console.log("Busqueda enviada");
    },
  },
};
</script>

<style scoped>
#menu {
  display: flex;
  background: beige;
}
ul {
  display: flex;
  list-style: none;
  font-size: 1.3rem;
  font-family: Arial, Helvetica, sans-serif;
  margin-top: 3rem;
  padding-right: 14rem;
}
ul li a {
  text-decoration: none;
  color: #11769e;
  font-weight: 700;
  padding-right: 4.8rem;
}
ul li a:hover {
  color: rgb(0, 0, 0);
  text-decoration: none;
  font-weight: 700;
}
form {
  padding: 0.7rem 0rem 0rem 2rem;
  display: flex;
  align-items: center;
}
input {
  margin: 1rem;
  padding: 0.5rem 1rem;
  border-style: solid;
  border: 2px solid #11769e;
  font-family: Arial, Helvetica, sans-serif;
  color: #181818;
  outline: none;
  line-height: 0.5rem;
  border-radius: 25px;
  font-size: 1rem;
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
.boton:hover {
  color: #11769e;
  background: rgb(29, 220, 226);
}
img {
  height: 5rem;
  width: 5rem;
}
</style>