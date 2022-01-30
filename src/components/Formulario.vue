<template>
  <div class="contact_form">
    <div class="formulario">
      <h1>Formulario de contacto</h1>
      <h3>Escríbenos y en breve los pondremos en contacto contigo</h3>
      <form action="submeter-formulario.php" method="post">
        <p>
          <label for="nombre" class="colocar_nombre"
            >Nombre
            <span class="obligatorio">*</span>
          </label>
          <input
            type="text"
            name="introducir_nombre"
            id="nombre"
            required="obligatorio"
            placeholder="Escribe tu nombre"
          />
        </p>
        <p>
          <label for="email" class="colocar_email"
            >Email
            <span class="obligatorio">*</span>
          </label>
          <input
            type="email"
            name="introducir_email"
            id="email"
            required="obligatorio"
            placeholder="Escribe tu Email"
          />
        </p>
        <p>
          <label for="asunto" class="colocar_asunto"
            >Asunto
            <span class="obligatorio">*</span>
          </label>
          <input
            type="text"
            name="introducir_asunto"
            id="assunto"
            required="obligatorio"
            placeholder="Escribe un asunto"
          />
        </p>

        <p>
          <label for="mensaje" class="colocar_mensaje"
            >Mensaje
            <span class="obligatorio">*</span>
          </label>
          <textarea
            name="introducir_mensaje"
            class="texto_mensaje"
            id="mensaje"
            required="obligatorio"
            placeholder="Deja aquí tu comentario..."
          ></textarea>
        </p>

        <button type="submit" name="enviar_formulario" id="enviar">
          <p>Enviar</p>
        </button>

        <p class="aviso">
          <span class="obligatorio"> * </span>los campos son obligatorios.
        </p>
      </form>
    </div>
  </div>
</template>
<script>
export default {
  name: "Formulario",
};
</script>
<style scoped>
body {
  height: 100%;
  font-family: Arial, Helvetica, sans-serif;
  background-color: #11769e;
}

.contact_form {
  width: 600px;
  height: auto;
  margin-left: 5rem;
  padding-top: 30px;
  padding-bottom: 20px;
  background-color: beige;
  padding-left: 30px;
}

input {
  background-color: #fbfbfb;
  width: 600px;
  height: 40px;
  border-radius: 5px;
  border-style: solid;
  border-width: 1px;
  border-color: #11769e;
  margin-top: 10px;
  padding-left: 10px;
}

textarea {
  background-color: #fbfbfb;
  width: 600px;
  height: 100px;
  border-radius: 5px;
  border-style: solid;
  border-width: 1px;
  border-color: #11769e;
  padding-left: 10px;
  padding-top: 15px;
}

label {
  display: block;
  float: center;
}

button {
  height: 45px;
  padding-left: 5px;
  padding-right: 5px;
  margin-bottom: 20px;
  margin-top: 10px;
  text-transform: uppercase;
  background-color: #11769e;
  border-color: #11769e;
  border-style: solid;
  border-radius: 10px;
  width: 600px;
  cursor: pointer;
}

button p {
  color: #fff;
}

span {
  color: #11769e;
}

.aviso {
  font-size: 13px;
  color: #0e0e0e;
}

h1 {
  font-size: 39px;
  text-align: letf;
  color: #11769e;
}

h3 {
  font-size: 16px;
  color: #11769e;
}

p {
  font-size: 14px;
  color: #11769e;
}
</style>