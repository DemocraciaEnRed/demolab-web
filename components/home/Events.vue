<template>
  <div class="event-container">
    <div class="container">
      <h1 class="has-text-centered section-title">
        Eventos
      </h1>
      <div class="events">
        <!-- <no-ssr>
          <b-datepicker
            v-model="selectedDate"
            inline
            :unselectable-days-of-week="[0, 6]"
          />
        </no-ssr> -->
        <div class="event-list">
          <!-- hay que modificar el componente event segun figma -->
          <Event />
          <Event />
          <Event />
          <Event />
        </div>
      </div>
      <div class="has-text-centered mt-6">
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
      selectedDate: new Date()
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
@media only screen and (max-width: 768px) {
  .events{
    flex-direction: column;
  }
  .event-container{
    display: flex;
    justify-content: center;
  }
  .event-list{
    flex-direction: column;
  }
  .dropdown.is-inline .dropdown-menu{
    display: flex;
    justify-content: center;
  }
}
</style>
