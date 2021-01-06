<template>
  <b-carousel>
    <b-carousel-item v-for="(carousel, i) in carousels" :key="i">
      <section :class="`hero is-medium is-${carousel.color}`">
        <div class="hero-body has-text-centered">
          <h1 class="title">
            {{ carousel.text }}
          </h1>
        </div>
      </section>
    </b-carousel-item>
  </b-carousel>
</template>

<script>
export default {
  name: 'Carrousell',
  data () {
    return {
      carousels: [
        { text: '¿Que es DemoLab?', color: 'primary' },
        { text: 'Evento proximo', color: 'info' },
        { text: 'Otro evento proximo', color: 'success' }
      ]
    }
  }
}
</script>
