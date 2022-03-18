<template>
  <section>
      <b-carousel :indicator-inside="true" :autoplay="true" class="m-0">
        <b-carousel-item v-for="(carousel, i) in carousels" :key="i">
          <section class="m-0">
            <div class="hero-body has-text-centered">
              <img :src="require(`@/assets/${carousel.foto}`)" alt="">
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
        { text: '¿Que es DemoLab?', color: 'primary', indicator: '¿Que es </br> <span>DemoLab?</span>', foto: 'demolab.png' },
        { text: 'Evento proximo', color: 'info', indicator: 'Nuestros </br> <span>Proyectos</span>', foto: 'proyectos.png' },
        { text: 'Otro evento proximo', color: 'success', indicator: 'Participación </br> <span>Ciudadana</span>', foto: 'participaciondemo.png' },
        { text: 'Otro evento proximo', color: 'success', indicator: 'Asamblea </br> <span>Ciudadana</span>', foto: 'asamblea.png' }
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
