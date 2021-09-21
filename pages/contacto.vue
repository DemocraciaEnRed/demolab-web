<template>
  <div class="section">
    <div class="container">
      <h1 class="has-text-centered">
        Contacta al Laboratorio de Innovación <br>del Concejo de Bogotá
      </h1>
      <h1 class="has-text-centered ">DEMOLAB</h1>
    </div>

    <h2 class="has-text-centered mt-6 mb-5 has-text-black">Registra tus datos para contactarte </h2>
    <div class="form-container">
      <div class="field mb-5">
        <label class="label">Nombre</label>
        <div class="control">
          <input class="input " type="text" placeholder="Nombre">
        </div>
      </div>
      <div class="field mb-5">
        <label class="label">Email</label>
        <div class="control has-icons-left has-icons-right">
          <input class="input is-danger" type="email" placeholder="Email input" value="hello@">
          <span class="material-icons">
            exclamation_bold
          </span>
        </div>
        <p class="help is-danger">This email is invalid</p>
      </div>
      <div class="field mb-5">
        <label class="label">Motivo de Contacto</label>
        <div class="control">
          <div class="select">
            <select>
              <option >Participación y Apertura</option>
              <option >Gestión del Conocimiento</option>
              <option >Otros</option>
            </select>
          </div>
        </div>
      </div>
      <div class="field is-grouped mb-5">
        <div class="control">
          <button class="boton secondary button is-link">Enviar</button>
        </div>
      </div>
    </div>
    <div class="has-text-centered mt-6">
      <a href="tel:+57+xxxxxxxx" class="has-text-centered boton primary mx-auto">
        <h3 >Si necesitas llamarnos, puedes hacerlo a través del +57+xxxxxxxx</h3>
      </a>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
  input, select{
    border-radius: 0 !important;
    border-color: #5c49ba !important;
  }
  select::after{
    border-color:#5c49ba
  }
  .form-container{
    max-width: 500px;
    margin: auto;
  }
  .control .boton{
    border-radius: 0;
  }
</style>
