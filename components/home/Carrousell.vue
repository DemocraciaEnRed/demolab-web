<template>
  <b-carousel :indicator-inside="false">
    <b-carousel-item v-for="(carousel, i) in carousels" :key="i">
      <section :class="`hero is-medium is-${carousel.color}`">
        <div class="hero-body has-text-centered">
          <h1 class="title">
            {{ carousel.text }}
          </h1>
        </div>
      </section>
    </b-carousel-item>
    <template slot="indicators"  slot-scope="props">
      <span class="custom-item" v-html="carousels[props.i].indicator"/>
    </template>
  </b-carousel>
</template>

<script>
export default {
  name: 'Carrousell',
  data () {
    return {
      carousels: [
        { text: '¿Que es DemoLab?', color: 'primary', indicator: '¿Que es </br> <span>DemoLab?</span>', img: 'Banner_demolab.png' },
        { text: 'Evento proximo', color: 'info', indicator: 'Evento </br> <span>proximo</span>', img: '' },
        { text: 'Otro evento proximo', color: 'success', indicator: 'Otro </br> <span>Evento</span>', img: '' }
      ]
    }
  }
}
</script>
