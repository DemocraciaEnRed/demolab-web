<template>
  <section>
    <div class="container">
      <div class="services">
        <div class="description">
          <h2>Servicios</h2>
          <span>Trabajamos para consolidar un Concejo más abierto, innovador y transparente, por eso constantemente estamos desarrollado herramientas, metodologías y nuevos espacios para que la ciudadanía incida y participe activamente en los asuntos distritales. </span>
          <br>
          <br>
          <Button :primary="true" />
        </div>
        <div class="tile is-ancestor">
          <div class="tile is-3">
            <Card :text="'Participación e Incidencia'" imag="~/assets/participacion_mano.png" :imgAlt="'imagen participacion e incidencia'" />
          </div>
          <div class="tile is-3">
            <Card :text="'Aceleración a la Innovación'" imag="~/assets/participacion_rayo.png" :imgAlt="'aceleracio na la innovacion'"/>
          </div>
          <div class="tile is-3">
            <Card :text="'Gestión del Conocimiento'" />
          </div>
        </div>
      </div>
    </div>
    <article class="celest">
      <div class="container">
        <div class="square column" >
                    <iframe
            src="https://player.vimeo.com/video/446827718"
            width="1152"
            height="348"
            frameborder="0"
          />
        </div>
        <div class="weird-card">
          <h2>¿Qué es DemoLab? </h2>
          <div class="weird-content">
            <span>
              CONOCE MÁS SOBRE EL LABORATORIO<br> DE CONCEJO ABIERTO DE BOGOTÁ
            </span>
            <Button :secondary="true" />
          </div>
        </div>
      </div>
    </article>
  </section>
</template>

<script>
import Card from '../Card.vue'
import Button from '../Button.vue'

export default {
  components: { Card, Button }
}
</script>

<style>
  .services{
    display: flex;
    flex-direction: row;
    justify-content: center;
    padding: 50px 0;
  }

  .services .description{
    padding: 0 10px;
    max-width: 300px;
  }
  .description h2{
    font-size: 40px;
    line-height: 45px;
    color: #5C49BA
  }
  .square{
    /* background-color: #ccc; */
    height: 300px;
    width: 50%;
    position: relative;
    top: -20px;
    left: -150px;
  }
  .celest{
    background-color: #d9d7ff;
    margin-top: 20px;
    padding: 20px;
    padding-bottom: 50px;
  }
  .celest .container{
    display: flex;
  }
  .weird-card{
    background-color: white;
    display: inline-block;
    border-left: 10px solid blue;
    height: 150px;
    position: relative;
    top: 50px;
    left: -220px;
    padding: 10px;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  }
  .weird-card .boton{
    position: relative;
    right: -40px;
  }
  .weird-card h2{
    font-size: 25px;
    line-height: 31px;
    color: black;
  }
  .weird-content{
    display: flex;
  }
  @media only screen and (max-width: 768px) {
    .celest{
      margin-top: 0;
    }
    .services{
      flex-direction: column;
    }
    .weird-card{
      display: block;
      height: auto;
      top: 0;
      left: 0;
    }
    .weird-content{
      flex-direction: column;
    }
    .weird-content .boton{
      right: 0;
    }
    .square{
      display: none;
    }
    .services .description{
      text-align: center;
      margin-bottom: 20px;
      max-width: none;
    }

  }
</style>
