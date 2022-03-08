<template>
<div class="card">
  <div class="card-image">
    <figure class="image">
      <img src="~assets/rendición-cuentas.png" alt="">
    </figure>
  </div>
  <div class="card-content">
     <div class="media-content">
        <p class="title is-4">{{fecha}}</p>
        <p class="subtitle is-3">{{ title }}</p>
      </div>
  </div>
  <div class="content">
    <p class="event-description">
      {{ description }}
    </p>
      <br>
      <!-- <time datetime="2016-1-1">11:09 PM - 1 Jan 2016</time> -->
  </div>
  <Button :fullwidth="true" :icon="'add'" :ccolor="color" />
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
  .card{
    max-width: 267px;
    max-height: 500px;
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
  }
</style>
