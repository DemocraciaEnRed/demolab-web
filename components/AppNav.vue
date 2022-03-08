<template>
  <div class="container">
    <b-navbar>
      <template slot="brand">
        <b-navbar-item tag="router-link" :to="{ path: '/' }">
          <img
            height="60"
            width="76"
            class="logo"
            src="/images/logo.png"
            alt="DemoLab logo"
          >
        </b-navbar-item>
      </template>
      <template slot="end">
        <nuxt-link to="/" class="navbar-item">
          Inicio
        </nuxt-link>
        <nuxt-link to="/que-es-demolab" class="navbar-item">
          ¿Que es demolab?
        </nuxt-link>
        <nuxt-link to="/servicios" class="navbar-item">
          Servicios y experiencias
        </nuxt-link>
        <nuxt-link to="/eventos" class="navbar-item">
          Eventos
        </nuxt-link>
        <nuxt-link to="/metodologias" class="navbar-item">
          Metodologias
        </nuxt-link>
        <!-- <nuxt-link to="/contacto" class="navbar-item">
          Contacto
        </nuxt-link> -->
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
  .navbar-brand{
    background-color: white;
  }
  .logo{
    max-height: 100px!important;
    height: 60px;
  }
  /* exact link will show the primary color for only the exact matching link */
  a.nuxt-link-exact-active {
    color: #00c58e;
  }

  @media screen and (max-width: 480) {
    .logo{
      height: 50px;
    }
  }
</style>
