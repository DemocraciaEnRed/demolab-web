<template>
  <div class="container about-us">
    <div class="has-text-centered about-title">
      <h3>Sobre nosotros</h3>
      <h1>¿Que es demolab?</h1>
      <p>DEMOLAB es el Laboratorio de Concejo Abierto de Bogotá <br>
      que trabaja para consolidar una corporación más abierta e innovadora en la ciudad. </p>
      <img height="250" width="450" src="~assets/reu.png" alt="?">
    </div>
    <div class="">
      <div class="columns  spacing">
        <div class="column mr-6 pr-6">
          <h1>¿Qué es el DemoLab?</h1>
            <p class="texto">
              El <b>DemoLab</b> es el Laboratorio de <b>Concejo Abierto de Bogotá</b>, es el primer laboratorio de innovación pública y gobierno abierto de una corporación en Colombia y uno de los pocos en América Latina y el mundo.<br><br>
              Tiene como objetivo <b>consolidar un Concejo de Bogotá abierto</b>, es decir más transparente, participativo y colaborativo e <b>innovador</b>, esto quiere decir que utiliza tecnología cívica centrada en la ciudadanía para que pueda aportar y nutrir los debates en el Concejo de la ciudad.
            </p>
        </div>
        <div class="column has-text-centered">
          <img src="~/assets/manos.png" alt="imagen con manos" class="ml-6 pl-6">
        </div>
      </div>
      <div class="columns spacing">
        <div class="column has-text-centered" style="position:relative;">
          <div  style="position:absolut; left:0px;">          <img src="~assets/agenda.png" alt="imagen de una agenda">
</div>
        </div>
        <div class="column has-text-right ml-6 pl-6">
          <h1>¿Cómo funciona?</h1>
          <p class="texto">
            El DemoLab tiene una metodología de trabajo que permite identificar los<br> procesos y actividades en los que puede <b>innovar</b>. Al igual genera<br> herramientas <b>metodológicas</b> y procesos de innovación dirigidos al interior<br> y la <b>ciudadanía</b> y generar estrategias que contribuyeb a la apertura e <br>innovación en el Concejo de Bogotá.<br> Por ello diseñó 3 líneas estratégicas de participación incidente <br><br> Linea de Apertura, Participación e Incidencia<br><br> Línea de Aceleración a la innovación <br><br>Línea de Gestión del Conocimiento</p>
        </div>
      </div>
      <div class="columns spacing">
        <div class="column">
          <h1>¿Para qué sirve?</h1>
          <p class="texto">
            El DemoLab nació de la necesidad de estructurar un modelo mixto de gobernanza que contribuya a la innovación democrática, incidencia y mecanismos de participación que acerque la ciudadanía a la corporación.<br><br>Esta apuesta por la innovación democrática es posible gracias a la visión de la mesa directiva de 2020, la continuidad, el liderazgo de la mesa de 2021 del Concejo de Bogotá y la alianza estratégica entre la Fundación Corona, el Extituto de Política Abierta, Ideemos, la Fundación Friedrich Ebert Stiftung (FESCOL), el Instituto Holandés para la Democracia Multipartidaria (NIMD), la Fundación Avina y Diseño Público
          </p>
        </div>
        <div class="column has-text-centered">
          <img src="~assets/foco.png" alt="">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AboutHeader'
}
</script>

<style>
.spacing{
  margin-bottom: 8rem !important;
}
.about-title{
  margin: 40px 0;
}
.about-title img, .about-title video{
  margin-top: 20px;
}
.texto{

  font-family: Raleway;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 19px;
  color: #000000;

}
</style>
