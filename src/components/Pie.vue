<template>
  <footer id="pie">
    <div>
      <a href="http://"
        ><img class="logo" src="../assets/logo.png" alt="logotipo"
      /></a>
    </div>
    <div>
      <p>infoweb © Copyright 2022 - All right reserved</p>
    </div>
    <div class="icono">
      <a href="https://www.gmail.com/mail/help/intl/es/about.html?iframe"
        ><img
          class="facebook"
          src="../assets/iconos/facebook.png"
          alt="facebook"
      /></a>
      <a href="https://www.gmail.com/mail/help/intl/es/about.html?iframe"
        ><img class="gmail" src="../assets/iconos/gmail.png" alt="gmail"
      /></a>
      <a href="https://web.whatsapp.com/"
        ><img
          class="whatsapp"
          src="../assets/iconos/whatsapp.png"
          alt="whatsapp"
      /></a>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Pie",
};
</script>

<style scoped>
#pie {
  display: flex;
  justify-content: space-between;
  background-color: #0f053d;
}
#pie p {
  font-family: Arial, Helvetica, sans-serif;
  font-weight: 700;
  color: white;
}
.icono {
  display: flex;
  justify-content: right;
}
.facebook {
  padding-right: 10px;
  padding-top: 8px;
  width: 2rem;
  height: 2rem;
}
.whatsapp {
  padding-right: 1rem;
  padding-top: 10px;
  width: 2rem;
  height: 2rem;
}
.gmail {
  padding-right: 1rem;
  width: 3rem;
  height: 3rem;
}
.logo {
  padding-left: 1rem;
  width: 3rem;
  height: 3rem;
}
</style>