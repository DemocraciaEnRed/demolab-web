<template>
  <div class="event">
    <h3 class="event-title text-center" v-bind:style="{ color: color }">
      <span class="material-icons">{{ icon }}</span>
      {{ title }}
    </h3>
    <p class="event-description">
      {{ description }}
    </p>
    <Button :fullwidth="true" :icon="'local_hospital'" :text="'detalles'" :customColor="color"/>
  </div>
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
    title: {
      type: String,
      default: 'Title'
    },
    icon: {
      type: String,
      default: 'ondemand_video'
    },
    description: {
      type: String,
      default: 'Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint.'
    }
  }
}
</script>

<style>
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
