<template>
  <div>
    <h1 class="has-text-centered">Nuestro ADN</h1>
    <!-- <b-carousel
     progress
     progress-type="is-primary"
     :icon-size="iconSize"
     :items-to-show="perList"
      :items-to-list="increment"
     :indicator="indicator"
     :auto-play="false"
     >
      <b-carousel-item v-for="(item, i) in items" :key="i" class="p-6">
        <section class="is-flex is-justify-content-center">
          <img :src="require(`@/assets/slide/${item.foto}`)" alt="">
        </section>
         <div class="carousel-indicator is-inside is-bottom">
          <a class="indicator-item"><span class="indicator-style is-dots" /></a><a class="indicator-item is-active"><span class="indicator-style is-dots" /></a><a class="indicator-item"><span class="indicator-style is-dots" /></a>
        </div>
      </b-carousel-item>
    </b-carousel> -->
    <b-carousel-list
            :data="items"
            :items-to-show="perList"
            :items-to-list="increment"
            :repeat="false"
            >
                <template #item="list" id="list.title">
                  <section class="is-flex is-justify-content-center">
                    <img :src="require(`@/assets/slide/${list.foto}`)" alt="">
                  </section>
                </template>
       </b-carousel-list>
  </div>
</template>

<script>
export default {
  name: 'Adn',
  mounted () {
    const resolution = window.screen.width
    if (resolution > 720) {
      this.perList = 2
    } else {
      this.perList = 1
    }
  },
  data () {
    return {
      iconSize: 'is-large',
      indicator: false,
      perList: 2,
      increment: 1,
      items: [
        { foto: 'aperturaA.png' },
        { foto: 'aperturaB.png' },
        { foto: 'participacionA.png' },
        { foto: 'participacionB.png' },
        { foto: 'incidenciaA.png' },
        { foto: 'incidenciaB.png' }
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
