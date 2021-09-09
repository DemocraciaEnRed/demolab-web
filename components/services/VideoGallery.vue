<template>
  <div class="video-gallery">
    <div class="container">
      <div class="columns main-video">
        <div class="column">
          <h1>Opini&oacute;n ciudadana</h1>
          <p>Uno de los grandes retos del laboratorio de innovación política DemoLab es  consolidar un Concejo de Bogotá abierto, es decir, participativo, colaborativo, transparente e innovador , que apoyado en tecnología civica logre incidir en las diferentes metodologías y las  decisiones que toma el Concejo de Bogotá.</p>
        </div>
        <div class="column">
          <iframe
            src="https://player.vimeo.com/video/446827718"
            width="640"
            height="360"
            frameborder="0"
          />
        </div>
      </div>
      <div class="columns list-videos">
        <div class="column video-item">
          <iframe
            src="https://player.vimeo.com/video/446827718"
            width="250"
            frameborder="0"
          />
          <h3 class="secondary-color">
            ¿Por qu&eacute; es tan importante demolab?
          </h3>
        </div>
        <div class="column video-item">
          <iframe
            src="https://player.vimeo.com/video/446827718"
            width="250"
            frameborder="0"
          />
          <h3 class="secondary-color">
            ¿Por qu&eacute; es tan importante demolab?
          </h3>
        </div>
        <div class="column video-item">
          <iframe
            src="https://player.vimeo.com/video/446827718"
            width="250"
            frameborder="0"
          />
          <h3 class="secondary-color">
            ¿Por qu&eacute; es tan importante demolab?
          </h3>
        </div>
        <div class="column video-item">
          <iframe
            src="https://player.vimeo.com/video/446827718"
            width="250"
            frameborder="0"
          />
          <h3 class="secondary-color">
            ¿Por qu&eacute; es tan importante demolab?
          </h3>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'VideoGallery'
}
</script>

<style scoped>
.video-gallery{
  background-color: #FAFAFA;
  padding: 50px 0;
}
.main-video{
  align-items: center;
}
.video-item{
  text-align: center;
}
</style>
