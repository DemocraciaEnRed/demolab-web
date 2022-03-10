<template>
  <div class="sucess-case">
    <h3 class="case-title text-center" :style="{ color: color }">
      {{ title }}
    </h3>
    <p class="case-description py-3">
      {{ description }}
    </p>
    <p v-if="readMore" class="case-description">
      {{ moreDescription }}
    </p>
    <button @click="showMore" v-if="!readMore" class="boton"><span class="mateirla-icons">Leer más</span></button>
    <button @click="showLess" v-if="readMore" class="boton"><span class="mateirla-icons">Leer Menos</span></button>
  </div>
</template>

<script>

export default {
  name: 'Case',
  props: {
    color: {
      type: String,
      default: '#5C49BA'
    },
    title: {
      type: String,
      default: 'Title'
    },
    description: {
      type: String,
      default: 'Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint.'
    },
    moreDescription: {
      type: String,
      default: 'Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint.'
    }
  },
  data: () => ({
    readMore: false
  }),
  methods: {
    showMore () {
      this.readMore = true
    },
    showLess () {
      this.readMore = false
    }
  }
}
</script>

<style>
  .sucess-case{
    height: 270px ;
    position: relative;
  }
  .event{
    background-color: white;
    margin: 0px 5px;
  }

  .case-title {
    margin-right: 15px;

    font-family: Staatliches;
    font-style: normal;
    font-weight: normal;
    font-size: 25px;
    line-height: 31px;

    color: #000000;

  }
  .case-description, .event-title{

    font-family: Raleway;
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 19px;
    padding-top: 20px;
    color: #090909;

  }
  .event-description{
    text-align: center;
  }
  .boton{
    margin-left:300px;
    position: absolute;
    right: 0px;
    bottom: 0px;
  }
</style>
