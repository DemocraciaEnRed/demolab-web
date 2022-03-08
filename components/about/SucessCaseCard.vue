<template>
  <div class="sucess-case">
    <h3 class="case-title text-center" :style="{ color: color }">
      {{ title }}
    </h3>
    <p class="case-description">
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
  .succes-case{
    width: 500px;
  }
  .event{
    background-color: white;
    margin: 0px 5px;
  }
  .event-title{
    display: flex;
    align-items: center;
  }
  .case-title span{
    margin-right: 15px;

    font-family: Staatliches;
    font-style: normal;
    font-weight: normal;
    font-size: 25px;
    line-height: 31px;

    color: #000000;

  }
  .event-description, .event-title{
    padding: 10px;

    font-family: Raleway;
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 19px;

    color: #090909;

  }
  .event-description{
    text-align: center;
  }
</style>
