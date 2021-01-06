<template>
  <div class="card">
    <div class="card-image">
      <figure class="image is-4by3">
        <img :src="img" :alt="imgAlt">
      </figure>
    </div>
    <div class="card-content">
      <div class="content">
        <strong> {{ text }} </strong>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    text: {
      type: String,
      default: 'Hola mundo'
    },
    img: {
      type: String,
      default: 'https://bulma.io/images/placeholders/1280x960.png'
    },
    imgAlt: {
      type: String,
      default: 'placeholder'
    }
  }
}
</script>

<style>
  .card{
    margin: 10px
  }
</style>
