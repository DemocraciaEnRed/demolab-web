<template>
  <div class="card p-0 m-0 card-config">
    <div class="card-image">
      <figure class="image">
        <img :src="require(`@/components/metodologies/image/${this.foto}`)" alt="">
      </figure>
    </div>
    <div class="card-content card-content-config has-text-centerer">
      <div class="media-content mc-config">
          <div class="subtitle is-4" :style="`color:${this.color} !important`"><p class="has-text-center">{{ title }}</p></div>
        </div>
      <div class="content c-config">
        <p class="pt-6 pb-6">
          {{ description }}
        </p>
          <br>
      </div>
    </div>
</div>

</template>

<script>

export default {
  name: 'Card',
  props: {
    description: {
      type: String,
      default: 'Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint.'
    },
    title: {
      type: String,
      default: 'Amet minim mollit'
    },
    foto: {
      type: String,
      default: '300.png'
    },
    color: {
      type: String,
      default: '#000'
    }
  }
}
</script>
<style scoped>
  .card-config{
    max-width: 340px;
  }
  .mc-config{
    font-family: 'Staatliches';
    font-style: normal;
    font-weight: 400;
    font-size: 25px !important;
    line-height: 31px;
    text-align: center;

    color: #000000;
  }
  .c-config{

    font-family: 'Raleway';
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 19px;
    align-items: left;
    text-align: left;
    color: #090909;

  }
</style>
