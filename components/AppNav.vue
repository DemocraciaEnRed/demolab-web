<template>
  <div class="container navFont">
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
      <template slot="start">
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
        <div></div>
      </template>
      <template slot="end">
        <b-navbar-item tag="router-link" :to="{ path: '/' }">
          <img
            height="60"
            width="100%"
            class="logo"
            src="~assets/consejo-bogota.png"
            alt="DemoLab logo"
          >
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
.navFont{
  font-family: Staatliches;
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 25px;
}
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
