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
          <Event
                  fecha="28 de Junio"
                  title="Rendición de Cuentas"
                  description="El Concejo de Bogotá realizó la primera Rendición de Cuentas de 2021 y se establecieron 4 fases de participación para que la ciudadanía participara activamente"
                  color="#76DB7A"
                  foto="rendicion-cuentas.png"/>
          <Event
                  fecha="25 de Agosto"
                  title="Toolkit de Genero"
                  description="El DemoLab junto a las organizaciones aliadas diseñó diferentes herramientas para incorporarlas en las funciones del Concejo de Bogotá"
                  color="#5C49BA"
                  foto="genero.png"/>
          <Event
                  fecha="10 de septiembre"
                  title="#LaRutaPOT"
                  description="Se diseñó e implementó la estrategia de participación para deliberar con la ciudadanía opiniones y recomendaciones sobre el POT (Plan de Ordenamiento Territorial)"
                  color="#5C49BA"
                  foto="POT.png"/>
          <Event
                  fecha="10 de Diciembre"
                  title="Cultura de la Innovación "
                  description="Desde agosto de 2021 se realizó transferencia de conocimiento para capacitar a las y los funcionarios en innovación pública"
                  color="#5FD1BC"
                  foto="innovacion.png"/>
          <!-- <Event fecha="25 de Agosto" title="Toolkit de Genero" description="El DemoLab junto a las organizaciones aliadas diseñó diferentes herramientas para incorporarlas en las funciones del Concejo de Bogotá" urlLink="algo" color="'#76DB7A'"/>
          <Event fecha="10 de septiembre" title="#LaRutaPOT" description="Se diseñó e implementó la estrategia de participación para deliberar con la ciudadanía opiniones y recomendaciones sobre el POT (Plan de Ordenamiento Territorial)" urlLink="algo" color="'#76DB7A'"/>
          <Event fecha="10 de Diciembre" title="Cultura de la Innovación" description="El Concejo de Bogotá realizó la primera Rendición de Cuentas de 2021 y se establecieron 4 fases de participación para que la ciudadanía participara activamente" urlLink="algo" color="'#76DB7A'"/> -->
        </div>
      </div>
      <!-- <div class="has-text-centered mt-6">
        <Boton :text="'ver todos los eventos'" />
      </div> -->
    </div>
  </div>
</template>

<script>
// import Boton from '../Button.vue'
import Event from './Event.vue'

export default {
  components: {
    Event
    // Boton
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
  margin: 80px;
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
