<template>
  <div class="success">
    <div class="container">
      <h1 class="my-6">Casos de exito</h1>
      <div class="columns">
        <div class="column success-card">
          <SucessCaseCard :color="'#000000'" :title="'Reconocimiento OCDE'" :description="'En 2021 la Organización de Cooperación y Desarrollo Económico OCDE, resaltó el modelo de Asamblea Ciudadana Itinerante realizada por el Concejo de Bogotá y diseñada e implementada por el DemoLab, como un caso de éxito en el fortalecimiento de la democracia deliberativa y éste, fue el único a nivel de una corporación público administrativa y el único en América Latina'" />
        </div>
        <div class="column success-card">
          <SucessCaseCard :color="'#000000'" :title="'Reconocimiento Universidad Externado'" :description="'Reconocimiento Universidad ExternadoEn 2021 La Universidad Externado de Colombia presentó un dossier sobre innovación pública e innovación social y la estrategia de participación diseñada e implementada por el DemoLab,  Concejo a la Casa fue tomada como el primer caso de demoracia por aleatoriedad en Colombia.'" />
        </div>
        <div class="column success-card">
          <SucessCaseCard :color="'#000000'" :title="'Alianza con Enfoque de Género '" :description="'En 2021 se realizó el lanzamiento de la Caja de Herramientas para incorporar el enfoque de género en el trabajo que desarrolla el Concejo de la ciudad. Esta Caja fue diseñada por el DemoLab y en colaboración con coordinadores de las bancadas temáticas en temas de equidad y mujer del Concejo de Bogotá, la Secretaría de la Mujer y delegadas de ONU Mujeres, NIMD y Extituto de Política Abierta.'" />
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
  margin-bottom: 15px;
  border-left: solid 20px #5C49BA;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}
</style>
