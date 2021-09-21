<template>
  <div class="success">
    <div class="container">
      <h1>Casos de exito</h1>
      <div class="columns">
        <div class="column success-card">
          <SucessCaseCard :title="'SERVICIO DE HABILITACIÓN A LA INNOVACIÓN'" :description="'Es la primera vez que se diseñó una metodología de innovación que permite a las Unidades de Apoyo Normativo (UAN) , Concejales y demás funcionarios llevar a cabo procesos de innovación, participación y apertura guiados por el equipo de Demolab.'" :moreDescription="'Para  una  estrategia de llevar a cabo este fortalecimiento, los equipo deben solicitar mediante un correo al Laboratorio para que identificar el reto a abordar, entender un problema de manera sistémica, co-diseñar los prototipos necesarios que permita superar  el reto identificado y hacer transferencia metodológica para que las UAN o los funcionarios de las diferentes dependencias del Concejo, implementen las soluciones y se fortalezcan los procesos internos.'" />
        </div>
        <div class="column success-card">
          <SucessCaseCard :title="'ASAMBLEA CIUDADANA '" :description="'Por primera vez el Concejo de Bogotá a través del laboratorio de innovación pública Demolab , realizó la primera Asamblea Ciudadana Itinerante de Bogotá. Este modelo de innovación deliberativa convocó a la ciudadanía de manera aleatoria, de diferentes estratos socioeconómicos, edades y localidades para entablar un diálogo directo e informado sobre los retos que afronta el Plan de Ordenamiento Territorial - POT .'" :moreDescription="'La Asamblea Ciudadana contó con una primera fase de foros con expertos y expertas sobre POT , posteriormente tuvo una etapa formativa a traves de formación sincrónica y asincrónica y el gran ejercicio de deliberación se realizó el 5 y 12 de diciembre de 2020.'" />
        </div>
        <div class="column success-card">
          <SucessCaseCard :title="'SERVICIO DE HABILITACIÓN A LA INNOVACIÓN '" :description="'Es la primera vez que se diseñó una metodología de innovación que permite a las Unidades de Apoyo Normativo - UAN , Concejales y demás funcionarios del Concejo están llevando a cabo procesos de innovación, participación y apertura guiados por el equipo de Demolab.'" :moreDescription="'Para  una  estrategia de llevar a cabo este fortalecimiento, los equipo deben solicitar mediante un correo al Laboratorio para que identificar el reto a abordar, entender un problema de manera sistémica, co-diseñar los prototipos necesarios que permita superar el reto identificado y hacer transferencia metodológica para que las UAN o los funcionarios de las diferentes dependencias del Concejo, implementen las soluciones y se fortalezcan los procesos internos.'" />
        </div>
        <div class="column success-card">
          <SucessCaseCard :title="'CONCEJO A LA CALLE'" :description="'En lo corrido del 2021, se han realizado 2 sesiones de Cabildo Abierto del Concejo de Bogotá, los días 8 y 25 de mayo, la primera en la Plaza de Bolivar y la segunda en el Portal de las Américas. La sesión abrio el espacio para que al rededor de 80 personas, algunos de ellos integrantes de organizaciones de la sociedad civil, e expusieran sus opiniones sobre la coyuntura actual generada por la pandemia y otros factores dificiles por los que atraviesa actualmente Colombia.'" :moreDescription="'Sesión Portal las Américas (Portal Resistencia) La iniciativa de la sesión del 25 de mayo fue precedida por varios concejales  y organizaciones defensoas de los derechos Humanos, de hecho a través de la plataforma de técnología cívica de Demolab se lanzó un Reto de Ciudad para que la ciudadanía planteara sus ideas y comentara las propuestas de las demás personas, para que, a través del Concejo de Bogotá,  se estructuren alternativas reales para soluciones concretas que pueda desarrollar el Gobierno de Bogotá y el Gobierno Nacional.'" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import SucessCaseCard from './SucessCaseCard.vue'

export default {
  name: 'SuccessCases',
  components: {
    SucessCaseCard
  }
}
</script>

<style>
.success{
  margin: 50px 0;
  background-color: #FAFAFA;
}
.success h1{
  font-size: 40px;
  text-align: left;
}
.success-card{
  background-color: white;
  height: max-content;
  margin: 5px;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}
</style>
