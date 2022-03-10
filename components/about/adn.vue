<template>
  <div>
    <b-carousel progress progress-type="is-primary">
      <b-carousel-item v-for="(item, i) in items" :key="i">
        <section>
          <img :src="require(`@/assets/slide/${item.foto}`)" alt="">
        </section>
      </b-carousel-item>
    </b-carousel>
  </div>
  <!-- <div class="section">
        <h1 class="has-text-centered">Nuestro ADN</h1>
        <div class="is-flex is-justify-content-center justy">
            <div class="container section columns">
                <div class="column">
                    <img src="~assets/apertura_a.png" alt="">
                </div>
                <div class="column">
                    <img src="~assets/apertura_b.png" alt="">
                </div>
            </div>
        </div>
    </div> -->
</template>

<script>
export default {
  name: 'Adn',
  data () {
    return {
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
</style>
