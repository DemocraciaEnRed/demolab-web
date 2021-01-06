<template>
  <div>
    <AboutHeader />
    <SuccessCases />
    <Glossary />
  </div>
</template>
<script>
import AboutHeader from '~/components/about/Header.vue'
import Glossary from '~/components/about/Glossary.vue'
import SuccessCases from '~/components/about/SuccessCases.vue'

export default {
  name: 'About',
  components: {
    AboutHeader,
    Glossary,
    SuccessCases
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
