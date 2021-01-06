<template>
  <div>
    <AppNav />
    <nuxt />
    <Footer />
  </div>
</template>

<script>
import AppNav from '~/components/AppNav.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    AppNav, Footer
  }
}
</script>
