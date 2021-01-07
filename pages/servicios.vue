<template>
  <div>
    <VideoGallery />
    <SuccessCases />
    <Projects />
  </div>
</template>

<script>
import VideoGallery from '~/components/services/VideoGallery.vue'
import SuccessCases from '~/components/services/SuccessCases.vue'
import Projects from '~/components/services/Projects.vue'

export default {
  name: 'Services',
  components: {
    VideoGallery,
    SuccessCases,
    Projects
  },
  head () {
    return {
      title: 'DemoLab - Servicios y experiencias',
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
