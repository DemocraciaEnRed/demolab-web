<template>
  <section>
      <b-carousel :indicator-inside="true" :autoplay="true" class="m-0">
        <b-carousel-item v-for="(carousel, i) in carousels" :key="i">
          <section class="m-0">
            <div class="hero-body has-text-centered">
              <a :href="`${carousel.link}`">
                <img :src="require(`@/assets/${carousel.foto}`)" alt="">
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
  data () {
    return {
      carousels: [
        { text: '¿Que es DemoLab?', color: 'primary', indicator: '¿Que es </br> <span>DemoLab?</span>', foto: 'demolab.png', link: '/que-es-demolab' },
        { text: 'Evento proximo', color: 'info', indicator: 'Nuestros </br> <span>Proyectos</span>', foto: 'proyectos.png', link: 'metodologias' },
        { text: 'Otro evento proximo', color: 'success', indicator: 'Participación </br> <span>Ciudadana</span>', foto: 'participaciondemo.png', link: 'https://participa.demolab.com.co/' }
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
