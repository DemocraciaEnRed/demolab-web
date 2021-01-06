<template>
  <div class="home">
    <Carrousell />
    <Services />
    <Participate />
    <Stats />
    <Events />
    <Metodologies />
  </div>
</template>

<script>
import Carrousell from '~/components/home/Carrousell.vue'
import Services from '~/components/home/Services.vue'
import Participate from '~/components/home/Participate.vue'
import Stats from '~/components/home/Stats.vue'
import Events from '~/components/home/Events.vue'
import Metodologies from '~/components/home/Metodologies.vue'

export default {
  name: 'Home',
  components: {
    Services,
    Carrousell,
    Participate,
    Stats,
    Events,
    Metodologies
  },
  head () {
    return {
      title: 'DemoLab - Concejo Abierto',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Concejo abierto'
        }
      ]
    }
  }
}
</script>
<style>
  .home{
    background-color: #FAFAFA;
  }
</style>
