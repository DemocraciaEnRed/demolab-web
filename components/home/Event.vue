<template>
<div class="card card-config">
  <div class="card-image">
    <figure class="image">
      <img :src="require(`@/assets/eventos/${this.foto}`)" alt="">
    </figure>
  </div>
  <div class="card-content card-content-config has-text-centered">
     <div class="media-content media-content-config">
        <div class="title is-4">{{fecha}}</div>
        <div class="subtitle is-4" :style="`color:${this.color} !important`"><p class="has-text-center">{{ title }}</p></div>
      </div>
    <div class="content content-config">
      <p class="event-description pb-6">
        {{ description }}
      </p>
        <br>
        <!-- <time datetime="2016-1-1">11:09 PM - 1 Jan 2016</time> -->
    </div>
  </div>

  <Button :fullwidth="true" :icon="'add'" :ccolor="`${this.color}`" :urlLink="'/metodologias'"/>
      <!-- <span class="material-icons">{{ icon }}</span> -->

</div>
  <!-- <div class=" card event">
    <h3 class="event-title text-center" :style="{ color: color }">
      <span class="material-icons">{{ icon }}</span>
      {{ title }}
    </h3>
    <p class="event-description">
      {{ description }}
    </p>
    <Button :fullwidth="true" :icon="'local_hospital'" :text="'detalles'" :custom-color="color" />
  </div> -->
</template>

<script>
import Button from '../Button.vue'

export default {
  name: 'Event',
  components: {
    Button
  },
  props: {
    color: {
      type: String,
      default: '#5C49BA'
    },
    fecha: {
      type: String,
      default: 'Title'
    },
    title: {
      type: String,
      default: 'Title'
    },
    foto: {
      type: String,
      default: '300.png'
    },
    icon: {
      type: String,
      default: 'add'
    },
    description: {
      type: String,
      default: 'sin descripcion'
    }
  }
}
</script>

<style>
  .card-config{
    max-width: 267px;
    min-height: 450px;
    -webkit-box-shadow: 5px 5px 14px 0px rgba(0,0,0,0.7);
    box-shadow: 5px 5px 14px 0px rgba(0,0,0,0.7);
  }
  .card-content-config{
    margin-bottom: 10px !important;
  }
  .media-content-config{
    height: 55px;
  }
  .content-config{
    height: 124px;
  }
  .event{
    background-color: white;
    margin: 0px 5px;
  }
  .event-title{
    display: flex;
    align-items: center;
  }
  .event-title span{
    margin-right: 15px;
  }
  .event-description, .event-title{
    padding: 10px;
  }
  .event-description{
    text-align: center;
    font-family: 'Raleway';
    font-style: normal;
    font-weight: 500;
    font-size: 14px;
    line-height: 20px;
  }
  @media only screen and (max-width: 768px) {
    .card-config{
      margin-bottom: 10px;
    }
  }
</style>
