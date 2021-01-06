<template>
  <div class="container">
    <b-navbar>
      <template slot="brand">
        <b-navbar-item tag="router-link" :to="{ path: '/' }">
          <img
            class="logo"
            src="/images/logo.png"
            alt="Demo lab, concejo abierto"
          >
        </b-navbar-item>
      </template>
      <template slot="end">
        <b-navbar-item :to="{ path: '/' }">
          Inicio
        </b-navbar-item>
        <b-navbar-item :to="{ path: '/' }">
          ¿Que es demolab?
        </b-navbar-item>
        <b-navbar-item :to="{ path: '/' }">
          Servicios y experiencias
        </b-navbar-item>
        <b-navbar-item :to="{ path: '/' }">
          Eventos
        </b-navbar-item>
        <b-navbar-item :to="{ path: '/' }">
          Metodologias
        </b-navbar-item>
        <b-navbar-item :to="{ path: '/' }">
          Contacto
        </b-navbar-item>
      </template>
    </b-navbar>
  </div>
</template>

<script>

export default {
  name: 'AppNav'
}

</script>

<style>
  .logo{
    max-height: 100px!important;
    height: 60px;
  }
  @media screen and (max-width: 480) {
    .logo{
      height: 50px;
    }
  }
</style>
