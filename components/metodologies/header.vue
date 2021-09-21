<template>
  <div class="container about-us">
    <div class="has-text-centered about-title">
    <h1>METODOLOGÍAS</h1>
    <p>Cada metodología esta orientada en la generaración de valor público, fortalecimiento institucional a través de procesos de innovación política y nuevos mecanismos de participación para que todos y todas incidan en las decisiones que toma el Concejo de Bogotá</p>
  </div>
  <div class="container">
    <h1>LÍNEA DE PARTICIPACIÓN E INCIDENCIA</h1>
    <p class="mb-6">La línea de participación, incidencia y apertura enfoca su trabajo en el diseño y desarrollo de herramientas, metodologías, espacios, tecnología cívica y habilitación de la incidencia ciudadana en los procesos de toma de decisión del Concejo</p>
    <div class="columns">
      <div class="column metodology-card mb-6">
        <Card :title="'CONCEJO A LA CASA'" :description="'Es un espacio participativo que consiste en fortalecer el debate entorno a un tema de la ciudad. en 2020, abrimos la discusión del Plan Distrital de Desarrollo presentado por la actual. Administración, a cientos de ciudadanos que fueron escogidos de manera aleatoria y en 2021 la conversación será entorno al POT'" />
      </div>
      <div class="column metodology-card mb-6">
        <Card :title="'ASAMBLEA CIUDADANA ITINERANTE'" :description="'Es un mecanismo de participación que ya se ha realizado en otros países y busca que la ciudadanía asuma un rol activo y presente soluciones y recomendaciones a los problemas públicos, éste es un modelo Itinerante es decir, que la planeación cuatrienal incorpora a esta lógica una ventaja frente a otras actividades de democracia deliberativa en el mundo.'" />
      </div>
      <div class="column metodology-card mb-6">
        <Card :title="'AGENDA CIUDADANA'" :description="'La plataforma cuenta con dos grandes funcionalidades, “Propuestas Ciudadanas” y “Consultas del Concejo” que podrán ser utilizadas por Concejales/as (y sus UAN), bancadas, comisiones, mesas directivas y la Junta de Voceros/as. Ambas funcionalidades se estructurarán a través de “Retos de ciudad”, los cuales corresponden a grandes categorías de participación.'" />
      </div>
    </div>
    <div class="columns">
        <div class="column metodology-card mb-6">
        <Card :title="'PLATAFORMA TECNOLÓGICA'" :description="'Desarrollo de tecnología cívica para la participación e incidencia ciudadana en las decisiones y procesos del Concejo de Bogotá. Esta tecnología permite que la ciudadanía pueda proponerle al Concejo agendas, debates, causas y proyectos para trabajar colectivamente'" />
        </div>
        <div class="column metodology-card mb-6">
        <Card :title="'PROPUESTAS CIUDADANAS'" :description="'Propuestas ciudadanas es una estrategia que funciona a través de la plataforma tecnológica de participación de DemoLab y permite que la ciudadanía pueda enviar propuestas sobre retos temáticos de ciudad.'" />
        </div>
        <div class="column metodology-card mb-6">
        <Card :title="'CONCEJO A LA CALLE'" :description="'Concejo a la Calle es una estrategia que le permite al Concejo sesionar de manera abierta en las calles de la ciudad, con una metodología de participación ciudadana que involucra mecanismos verbales, escritos, tecnológicos, entre otros'" />
      </div>
    </div>
  </div>
  <div class="container">
    <h1 class="mt-6 mb-3">LÍNEA DE ACELERACIÓN A LA INNOVACIÓN </h1>
    <div class="columns">
      <div class="column metodology-card mb-6">
        <Card :title="'SERVICIO DE HABILITACIÓN A LA INNOVACIÓN'" :description="'Utiliza metodologías de pensamiento de diseño y de pensamiento sistémico con el objetivo de que asesoras, asesores, funcionarios, funcionarias, concejales y concejalas, puedan encontrar soluciones innovadoras a problemas y retos de la Corporación y la ciudad'" />
      </div>
      <div class="column metodology-card mb-6">
        <Card :title="'CAJA DE HERRAMIENTAS PARA LA TRANSVERSALIZACIÓN DEL ENFOQUE DE GÉNERO'" :description="'Esta caja de herramientas fue co-creada entre el Concejo de Bogotá (Mesa Directiva año 2020), el DemoLab, la Secretaría Distrital de la Mujer, ONU Mujeres, el Instituto Holandés para la Democracia Multipartidista (NIMD) y Extituto de Política Abierta, la Bancada Bancada para la Equidad de la mujer, el Sistema Distrital de Cuidado y Eliminación de todas las Violencias Basadas en Género, y la Bancada de la Mujer. Este instrumento, permite a los y las Concejalas y sus equipos transversalizar el enfoque de género en. proyectos de acuerdo normativo, debates de control político, y  presupuesto de la ciudad.'" />
      </div>
      <div class="column metodology-card mb-6">
        <Card :title="'CULTURA DE LA INNOVACIÓN'" :description="'El DemoLab ha diseñado una estrategia para fortalecer las capacidades de innovación en funcionarios y funcionarias en el Concejo de Bogotá. Esta estrategia tiene elementos y procesos de transferencias metodológicas, sistemas de incentivos para la apropiación de la innovación, momentos de intercambio de aprendizajes con miembros del ecosistema de gobierno abierto, innovación pública, entre otros.'" />
      </div>
    </div>
  </div>
  <div class="container">
    <h1 class="mt-6 mb-3">GESTIÓN DEL CONOCIMIENTO</h1>
    <div class="columns">
      <div class="column metodology-card mb-6">
        <Card :title="'SERVICIO DE HABILITACIÓN A LA INNOVACIÓN'" :description="'Utiliza metodologías de pensamiento de diseño y de pensamiento sistémico con el objetivo de que asesoras, asesores, funcionarios, funcionarias, concejales y concejalas, puedan encontrar soluciones innovadoras a problemas y retos de la Corporación y la ciudad'" />
      </div>
      <div class="column metodology-card mb-6">
        <Card :title="'CAJA DE HERRAMIENTAS PARA LA TRANSVERSALIZACIÓN DEL ENFOQUE DE GÉNERO'" :description="'Esta caja de herramientas fue co-creada entre el Concejo de Bogotá (Mesa Directiva año 2020), el DemoLab, la Secretaría Distrital de la Mujer, ONU Mujeres, el Instituto Holandés para la Democracia Multipartidista (NIMD) y Extituto de Política Abierta, la Bancada Bancada para la Equidad de la mujer, el Sistema Distrital de Cuidado y Eliminación de todas las Violencias Basadas en Género, y la Bancada de la Mujer. Este instrumento, permite a los y las Concejalas y sus equipos transversalizar el enfoque de género en. proyectos de acuerdo normativo, debates de control político, y  presupuesto de la ciudad.'" />
      </div>
      <div class="column metodology-card mb-6">
        <Card :title="'CULTURA DE LA INNOVACIÓN'" :description="'El DemoLab ha diseñado una estrategia para fortalecer las capacidades de innovación en funcionarios y funcionarias en el Concejo de Bogotá. Esta estrategia tiene elementos y procesos de transferencias metodológicas, sistemas de incentivos para la apropiación de la innovación, momentos de intercambio de aprendizajes con miembros del ecosistema de gobierno abierto, innovación pública, entre otros.'" />
      </div>
    </div>
  </div>
</div>
</template>

<script>
import Card from './Card.vue'
export default {
  name: 'MetodologiesHeader',
  components: {
    Card
  }
}
</script>

<style>
.about-title{
  margin: 40px 0;
}
.about-title img, .about-title video{
  margin-top: 20px;
}
.metodology-card{
  background-color: white;
  height: max-content;
  margin: 5px;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}
</style>
