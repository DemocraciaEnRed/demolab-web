<template>
  <div>
    <b-carousel progress progress-type="is-primary" :icon-size="iconSize" :indicator="indicator" :auto-play="false">
      <b-carousel-item v-for="(item, i) in items" :key="i" class="p-6">
        <section class="is-flex is-justify-content-center">
          <img :src="require(`@/assets/slide/${item.foto}`)" alt="">
        </section>
        <!-- <div class="carousel-indicator is-inside is-bottom">
          <a class="indicator-item"><span class="indicator-style is-dots" /></a><a class="indicator-item is-active"><span class="indicator-style is-dots" /></a><a class="indicator-item"><span class="indicator-style is-dots" /></a>
        </div> -->
      </b-carousel-item>
    </b-carousel>
  </div>
</template>

<script>
export default {
  name: 'Adn',
  data () {
    return {
      iconSize: 'is-large',
      indicator: false,
      items: [
        { foto: 'apertura.png' },
        { foto: 'participacion.png' },
        { foto: 'incidencia.png' }
      ]
    }
  }
}
</script>

<style scoped>
.justy {
  margin-left: 100px;
}
.carousel .carousel-indicator{
  display: none !important;
}
.carousel-arrow .icon .has-icons-left, .carousel-arrow .icon .has-icons-right{
  background-color: #584DB3 !important;
  color: #584DB3 !important;
}
</style>
