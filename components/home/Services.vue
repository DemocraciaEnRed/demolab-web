<template>
  <section class="center mt-6">
    <div class="container">
      <div class="services">
        <div class="description">
          <h2>Servicios</h2>
          <span>Trabajamos para consolidar un Concejo más abierto, innovador y transparente, por eso constantemente estamos desarrollado herramientas, metodologías y nuevos espacios para que la ciudadanía incida y participe activamente en los asuntos distritales. </span>
          <br>
          <br>
          <Button :primary="true" :urlLink="'/servicios'" :ccolor="'#5fd1bc'"/>
        </div>
        <div class="tile is-ancestor is-flex is-justify-content-center">
          <div class="tile is-parent">
                      <div class="card card-height is-child mx-6">
            <div class="image">
              <img src="~/assets/participacion_mano.png" alt="imagen participacion e incidencia">
            </div>
            <div class="title is-4 has-text-centered mt-3">Participación e Incidencia</div>
          </div>
          <div class="card card-height is-child mx-6">
            <div class="image">
              <img src="~/assets/participacion_rayo.png" alt="aceleracio na la innovacion">
            </div>
            <div class="title is-4 has-text-centered mt-3">Aceleración a la Innovación</div>
          </div>
          <div class="card card-height is-child mx-6">
            <div class="image">
              <img src="~/assets/gestion_foco.png" alt="gestion del conocimiento">
            </div>
            <div class="title is-4 has-text-centered mt-3">Gestión del Conocimiento</div>
          </div>
          </div>
        </div>
      </div>
    </div>
    <article class="celest">
      <div class="container mb-6 pb-6">
        <div class="square" >
                    <iframe
            src="https://www.youtube.com/embed/Q5FYG8Iy_KM"
            width="550"
            height="348"
            frameborder="0"
          />
        </div>
      <div class="weird-card  weird-content-config">
          <h2 class="mb-3">¿Qué es DemoLab? </h2>
          <div class="weird-content">
            <span>
              CONOCE MÁS SOBRE EL LABORATORIO<br> DE CONCEJO ABIERTO DE BOGOTÁ
            </span>
            <div class="boton-config">
              <Button  :secondary="true" />
            </div>
          </div>
      </div>
      </div>
    </article>
    <section class="to-mobile">
       <div class="square-mobile column" >
          <iframe
            src="https://www.youtube.com/embed/Q5FYG8Iy_KM"
            width="250"
            height="348"
            frameborder="0"
          />
        </div>
        <div class="weird-card mb-6">
          <h2 class="mb-3">¿Qué es DemoLab? </h2>
          <div class="weird-content weird-content-config-mobile">
            <span>
              CONOCE MÁS SOBRE EL LABORATORIO<br> DE CONCEJO ABIERTO DE BOGOTÁ
            </span>
            <div class="boton-config-mobile">
              <Button  :secondary="true" :fullwidth="true"/>
            </div>
          </div>
      </div>
    </section>
  </section>
</template>

<script>
// import Card from '../Card.vue'
import Button from '../Button.vue'

export default {
  components: { Button }
}
</script>

<style>
    .card-height{
      height: 80% ;
    }
.title{
  font-weight: normal !important;
}
  /* .center{
    margin-left: 50px;
  } */
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
    top: -18px;
    left: 170px;
  }
  .to-mobile{
    visibility: hidden ;
    display: none;
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
    border-left: 10px solid #5c49ba;
    height: 150px;
    width: 455px;
    padding: 10px;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  }
  .boton-config{
    position: absolute !important;
    right: -35px !important;
    bottom: 30px !important;
  }
  .weird-content-config{
    position: relative;
    top:70px;
    left: -120px;
  }
  .weird-card h2{
    font-size: 25px;
    line-height: 31px;
    color: black;
  }
  .weird-content{
    display: flex;
  }
  @media only screem and (min-width: 950px){
    .card-height{
      height: 80% ;
    }
  }
  @media only screen and (min-with: 769px) and (max-with: 1215px){
    .celest{
      margin-top: 50px;
    }
    .square{
      position: relative;
      top: -30px;
      left: 0px;
    }
    .weird-content-config{
      top: 70px;
      left: -286px;
    }
  }
  @media only screen and (max-width: 768px) {
    .card-height{
      height: auto ;
    }
    .celest{
      margin-top: 0;
      display: none;
    }
    .services{
      flex-direction: column;
    }
    .weird-card{
      display: block;
      height: auto;
      width: auto;
      top: 0;
      left: 0;
    }
    .weird-content-config{
      position: absolute;
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
    .to-mobile{
      visibility: visible;
      display: block;

    }
    .square-mobile{
      visibility: visible;
      display: block;
    }
    iframe{
      width: 100%;
    }
    .weird-content-config-mobile{
      position: relative;
    }
    .boton-config-mobile{
      position: relative;
    }
    .services .description{
      text-align: center;
      margin-bottom: 20px;
      max-width: none;
    }

  }
</style>
