<template>
  <div>
    <!-- <VideoGallery /> -->
    <!-- <SuccessCases />
    <Projects /> -->
    <allPage />
  </div>
</template>

<script>
// import VideoGallery from '~/components/services/VideoGallery.vue'
// import SuccessCases from '~/components/services/SuccessCases.vue'
// import Projects from '~/components/services/Projects.vue'
import allPage from '~/components/services/all.vue'
export default {
  name: 'Services',
  components: {
    // VideoGallery,
    allPage
    // SuccessCases,
    // Projects
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
