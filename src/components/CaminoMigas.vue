<template>
  <section id="camino-migas">
    <div class="migas">
      <a href="#"> Inicio </a> / <a href="#">Covid </a> /
      <a href="#" class="actual">Vacunas</a>
    </div>
    <div class="grupo">
      <div class="dropdown">
        <button class="dropbtn">INICIAR SESIÓN</button>
        <div class="dropdown-content">
          <button class="tw">Login</button>
          <button class="fb">Facebook</button>
          <button class="correo">Gmail</button>
        </div>
      </div>
      <a href="#">REGISTRO</a>
    </div>
  </section>
</template>

<script>
export default {
  name: "CaminoMigas",
};
</script>

<style scoped>
#camino-migas {
  margin-left: 1rem;
  display: flex;
  justify-content: space-between;
  color: #11769e;
}

a:hover {
  color: rgb(0, 0, 0);
}

a {
  text-decoration: none;
  font-size: 1.2rem;
  margin: 0 1rem 0 1rem;
  color: #11769e;
}

.migas {
  margin-top: 4rem;
}

.grupo {
  margin-top: 1rem;
  padding: 0 1rem 0 1rem;
  font-weight: 700;
}
.dropbtn {
  color: #11769e;
  padding: 16px;
  font-size: 1.2rem;
  border: none;
  font-weight: 700;
  background-color: beige;
}
.dropbtn :hover {
  color: black;
}
.dropdown {
  position: relative;
  display: inline-block;
}
.dropdown-content {
  display: none;
  position: absolute;
  min-width: 1rem;
  z-index: 1;
}
.dropdown-content i {
  text-decoration: none;
  display: block;
}
.dropdown:hover .dropdown-content {
  display: block;
}
button {
  width: 100%;
  padding: 10px;
  cursor: pointer;
  position: relative;
  margin-top: 10px;
  font-size: 1.2rem;
}
.fb {
  background: #3b5999;
  border-style: none;
  color: white;
  font-weight: 700;
}
.tw {
  background-color: beige;
  border-style: none;
  color: #11769e;
  font-size: 1.2rem;
  border: none;
  font-weight: 700;
}
.correo {
  background-color: rgb(231, 10, 10);
  border-style: none;
  color: white;
  font-weight: 700;
}
</style>