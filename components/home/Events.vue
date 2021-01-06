<template>
  <div class="event-container">
    <div class="container">
      <h1 class="has-text-centered section-title">
        Eventos
      </h1>
      <div class="events">
        <b-datepicker
          v-model="date"
          inline
          :unselectable-days-of-week="[0, 6]"
        />
        <div class="event-list">
          <Event />
          <Event />
          <Event />
          <Event />
        </div>
      </div>
      <div class="has-text-centered">
        <Boton :text="'ver todos los eventos'" />
      </div>
    </div>
  </div>
</template>

<script>
import Boton from '../Button.vue'
import Event from './Event.vue'

export default {
  components: {
    Event,
    Boton
  },
  data () {
    return {
      date: new Date()
    }
  }
}
</script>

<style>
.event-container{
  background-color: #FAFAFA;
  padding: 30px 0;
}
.events{
  display: flex;
  flex-direction: row;
}
.event-list{
  display: flex;
  flex-direction: row;
  align-items: center;
  align-content: space-between;
  margin-left: 5px;
}

</style>
