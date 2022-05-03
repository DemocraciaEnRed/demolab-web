<template>
  <section>
      <b-carousel :indicator-inside="true" :autoplay="true" class="m-0 hero is-medium-mobile">
        <b-carousel-item v-for="(carousel, i) in carousels" :key="i">
          <section v-if="divice" class="m-0">
            <div class="hero-body has-text-centered">
              <a :href="`${carousel.link}`">
                <img :src="require(`@/assets/${carousel.foto}`)" alt="">
             </a>
            </div>
          </section>
          <section v-else class="m-0">
            <div class="hero-body has-text-centered">
              <a :href="`${carousel.link}`">
                <img :src="require(`@/assets/${carousel.fotoMobile}`)" alt="">
             </a>
            </div>
          </section>
        </b-carousel-item>
        <template class="" slot="indicators"  slot-scope="props">
          <span class="custom-item" v-html="carousels[props.i].indicator"/>
        </template>
    </b-carousel>
  </section>
</template>

<script>
export default {
  name: 'Carrousell',
  beforeMount () {
    if (window.screen.width > 720) {
      this.divice = true
    } else {
      this.divice = false
    }
    console.log('screen: ', this.divice)
  },
  data () {
    return {
      divice: true,
      carousels: [
        { text: '¿Que es DemoLab?', color: 'primary', indicator: '¿Que es </br> <span>DemoLab?</span>', foto: 'demolab.png', fotoMobile: 'ejemplo.png', link: '/que-es-demolab' },
        { text: 'Evento proximo', color: 'info', indicator: 'Nuestros </br> <span>Proyectos</span>', foto: 'proyectos.png', fotoMobile: 'ejemplo.png', link: 'metodologias' },
        { text: 'Otro evento proximo', color: 'success', indicator: 'Participación </br> <span>Ciudadana</span>', foto: 'participaciondemo.png', fotoMobile: 'ejemplo.png', link: 'https://participa.demolab.com.co/' }
      ]
    }
  }
}
</script>
<style scoped>
  .relative{
    position: relative;
  }
  .absolute{
    position: absolute;
    bottom: 0px;
    right: 0px;
  }
</style>
