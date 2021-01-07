<template>
  <div class="video-gallery">
    <div class="container">
      <div class="columns main-video">
        <div class="column">
          <h1>Opini&oacute;n ciudadana</h1>
          <p>Aliqua id fugiat nostrud irure ex duis ea quis id quis ad et. Sunt qui esse pariatur duis deserunt mollit dolore cillum minim tempor enim. Elit aute irure tempor cupidatat incididunt sint deserunt ut voluptate aute id deserunt nisi.</p>
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
