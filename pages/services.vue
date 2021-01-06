<template>
  <div>
    <VideoGallery />
  </div>
</template>

<script>
import VideoGallery from '~/components/services/VideoGallery.vue'

export default {
  name: 'Services',
  components: {
    VideoGallery
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
