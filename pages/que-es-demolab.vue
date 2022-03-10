<template>
  <div>
    <AboutHeader />
    <SuccessCases />
    <!-- <Glossary /> -->
    <Adn />
    <Metodologies />
  </div>
</template>
<script>
import AboutHeader from '~/components/about/Header.vue'
// import Glossary from '~/components/about/Glossary.vue'
import SuccessCases from '~/components/about/SuccessCases.vue'
import Metodologies from '~/components/about/Metodologies.vue'
import Adn from '~/components/about/adn.vue'
export default {
  name: 'About',
  components: {
    AboutHeader,
    // Glossary,
    SuccessCases,
    Metodologies,
    Adn
  },
  head () {
    return {
      title: 'DemoLab - ¿Que es DemoLab?',
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

</style>
