<template>
  <div class="about-us has-text-centered">
    <div class="mb-6 pb-6 has-text-centered about-title">
      <h1>Opinión ciudadana</h1>
      <div class="container container-config has-text-centered">
        <p class="short-dec">Cada metodología está orientada fortalecer la confianza entre la ciudadanía y el Concejo mediante la apertura, la participación ciudadana, y la innovación.</p>
      </div>
    </div>
    <div class="container is-justify-content-center">
      <h1>LÍNEA DE PARTICIPACIÓN E INCIDENCIA</h1>
        <div class="container container-config has-text-centered">
          <p class="short-dec mb-6 ">La línea de participación, incidencia y apertura enfoca su trabajo en el diseño y desarrollo de herramientas, metodologías, espacios, tecnología cívica y habilitación de la incidencia ciudadana en los procesos de toma de decisión del Concejo</p>
        </div>
    </div>
    <section class="container container-config has-text-centered">
      <masonry-wall :items="participacion" :ssr-columns="3" :column-width="300" :gap="6">
        <template v-slot:default="{ item }">
          <div class="m-3">
              <Card :foto="`${item.foto}`" :title="`${item.title}`" :description="`${item.description}`" />
          </div>
        </template>
     </masonry-wall>
    </section>
    <div class="has-background-white">
      <div class="container is-justify-content-center">
        <h1 class="mt-6 mb-3">LÍNEA DE ACELERACIÓN A LA INNOVACIÓN </h1>
      </div>
      <section class="container container-config has-text-centered ">
        <masonry-wall :items="aceleracion" :ssr-columns="3" :column-width="300" :gap="6">
          <template v-slot:default="{ item }">
            <div class="m-3">
                <Card :foto="`${item.foto}`" :title="`${item.title}`" :description="`${item.description}`" />
            </div>
          </template>
      </masonry-wall>
      </section>
    </div>
    <div class="container  is-justify-content-center">
      <h1 class="mt-6 mb-3">GESTIÓN DEL CONOCIMIENTO</h1>
      <div class="container container-config has-text-centered">
          <p class="mb-6">La línea de participación, incidencia y apertura enfoca su trabajo en el diseño y desarrollo de herramientas, metodologías, espacios, tecnología cívica y habilitación de la incidencia ciudadana en los procesos de toma de decisión del Concejo</p>
        </div>
    </div>
    <section class="container container-config has-text-centered">
      <masonry-wall :items="conocimiento" :ssr-columns="3" :column-width="300" :gap="6">
        <template v-slot:default="{ item }">
          <div class="m-3">
              <Card :foto="`${item.foto}`" :title="`${item.title}`" :description="`${item.description}`" />
          </div>
        </template>
     </masonry-wall>
    </section>
  </div>
</template>

<script>
import MasonryWall from 'vue-masonry-wall'

import Card from './Card.vue'

export default {
  name: 'MetodologiesHeader',
  components: {
    Card,
    MasonryWall
  },
  data () {
    return {
      participacion: [
        { title: 'CONCEJO A LA CASA', description: 'Diseñamos y desarrollamos herramientas, proyectos, actividades, tecnología cívica y habilitación de la incidencia ciudadana en los procesos de toma de decisión del Concejo de Bogotá', foto: 'RutaPOT.png' },
        { title: 'ASAMBLEA CIUDADANA ITINERANTE', description: 'Es un mecanismo de participación que ya se ha realizado en otros países y busca que la ciudadanía asuma un rol activo y presente soluciones y recomendaciones a los problemas públicos, éste es un modelo Itinerante es decir, que la planeación cuatrienal incorpora a esta lógica una ventaja frente a otras actividades de democracia deliberativa en el mundo. Este modelo recibió en 2021 por parte de la OCDE, el reconocimiento como caso de éxito en el fortalecimiento de la democracia deliberativa.', foto: 'Asamblea.png' },
        { title: 'AGENDA CIUDADANA', description: 'La plataforma cuenta con dos grandes funcionalidades, “Propuestas Ciudadanas” y “Consultas del Concejo” que podrán ser utilizadas por Concejales/as (y sus UAN), bancadas, comisiones, mesas directivas y la Junta de Voceros/as. Ambas funcionalidades se estructurarán a través de “Retos de ciudad”, los cuales corresponden a grandes categorías de participación.', foto: 'AgendaCiudadana.png' },
        { title: 'PLATAFORMA TECNOLÓGICA', description: 'Desarrollo de tecnología cívica para la participación e incidencia ciudadana en las decisiones y procesos del Concejo de Bogotá. Esta tecnología permite que la ciudadanía pueda proponerle al Concejo agendas, debates, causas y proyectos para trabajar colectivamente', foto: 'PlataformaTecnologica.png' },
        { title: 'PROPUESTAS CIUDADANAS', description: 'Propuestas ciudadanas es una estrategia que funciona a través de la plataforma tecnológica de participación de DemoLab y permite que la ciudadanía envíe propuestas sobre retos temáticos de ciudad.', foto: 'PropuestasCiudadanas-01.png' },
        { title: 'CONCEJO A LA CALLE', description: 'Concejo a la Calle es una estrategia que le permite al Concejo sesionar de manera abierta en las calles de la ciudad, con una metodología de participación ciudadana que involucra mecanismos verbales, escritos, tecnológicos, entre otros', foto: 'ConcejoALaCasa.png' }

      ],
      aceleracion: [
        { title: 'SERVICIO DE HABILITACIÓN A LA INNOVACIÓN', description: 'Bogotá, para llevar a cabo procesos de innovación, participación y apertura guiados por el equipo de DemoLab. Este servicio apoya a los equipos de las y los concejales y funcionarios a identificar el reto a abordar, comprender su naturaleza, entender el problema y acompañar el proceso para que sean las y los funcionarios, asesores y/o concejales quienes implementen las soluciones creadas en este servicio.', foto: 'ServicioHabilitacionInnovacion.png' },
        { title: 'TOOLKIT DE GÉNERO', description: 'Esta caja de herramientas fue diseñada por el DemoLab en colaboración con la Secretaría Distrital de la Mujer, ONU Mujeres, el Instituto Holandés para la Democracia Multipartidista (NIMD) y Extituto de Política Abierta, la Bancada Bancada para la Equidad de la mujer, el Sistema Distrital de Cuidado y Eliminación de todas las Violencias Basadas en Género, y la Bancada de la Mujer. Este instrumento, permite a los y las Concejalas y sus equipos incluir el enfoque de género en.los proyectos de acuerdo normativo, debates de control político, y presupuesto de la ciudad.', foto: 'ToolkitGenero.png' },
        { title: 'CULTURA DE LA INNOVACIÓN', description: 'El DemoLab ha diseñado una estrategia para fortalecer las capacidades de innovación en funcionarios y funcionarias en el Concejo de Bogotá. Esta estrategia tiene elementos y procesos de transferencia metodológica, sistemas de incentivos para la apropiación de la innovación, momentos de intercambio de aprendizajes con miembros del ecosistema de gobierno abierto, innovación pública, entre otros.', foto: 'CulturaInnovacion.png' }
      ],
      conocimiento: [
        { title: 'PILOTO DE GESTIÓN DEL CONOCIMIENTO', description: 'Se realizará la identificación de un Piloto para la caracterización de fuentes, captura y recopilación de información bajo los lineamientos del ciclo de gestión del conocimiento con el fin de validar como se encuentra actualmente esta información establecida en las tablas de retención documental y determinar si es necesaria su actualización de acuerdo a la documentación que se genera en el área de planeación.', foto: 'PilotoGestionConocimiento.png' },
        { title: 'ARTICULACIÓN CON PLANEACIÓN PARA LA IMPLEMENTACIÓN DE MIPG', description: 'Es un acompañamiento en la implementación de la dimensión de Innovación y Gestión del Conocimiento de MIPG y en la estrategia de comunicación para la divulgación de la metodología y la importancia de la misma, así como la construcción de la narrativa y apropiación de la gestión del conocimiento al interior del Concejo.', foto: 'ArticulacionMIPG.png' },
        { title: 'ACERCAMIENTO Y VINCULACIÓN A ESPACIOS ACADÉMICOS Y DE INVESTIGACIÓN', description: 'Acercamiento, relacionamiento y vinculación a instituciones o centros académicos y de investigación para co-crear conocimiento por medio de procesos de experimentación, proyección, innovación, prospección e investigación que permita la generación de valor público a la corporación.', foto: 'AcercamientoEspaciosAcademicos.png' },
        { title: 'ARTICULACIÓN CON LOS SISTEMAS DE GESTIÓN DE CONOCIMIENTO E INNOVACIÓN', description: 'Vinculación con los diferentes actores, centros de pensamientos, observatorios que hacen parte del ecosistema de innovación de Bogotá y Colombia para crear sinergias que fortalezcan la innovación y gestión del conocimiento de la corporación y la generación de valor público.', foto: 'ArticulacionSistemasDeGestion.png' },
        { title: 'CAJA DE HERRAMIENTAS PARA LA TRANSVERSALIZACIÓN DEL ENF', description: 'Herramienta que permite identificar el conocimiento con que cuentan las personas, entidades u organizaciones con el fin de desarrollar de manera conjunta actividades o proyectos que permitan mejorar las capacidades de la corporación, así como tener a disposición los mecanismos de conservación de gestión del conocimiento.', foto: 'MapasGestionConocimiento-01.png' },
        { title: 'SISTEMATIZACIÓN DE LECCIONES APRENDIDAS Y BUENAS PRÁCTICAS DEL CONCEJO DE BOGOTÁ', description: 'El fortalecimiento de las entidades públicas como lo establece el Departamento Administrativo de la Función Pública, se encuentra estrechamente relacionado con la gestión documental, ya que esta permite recopilar, sistematizar y administrar la información de tal manera que respalde la evidencia de la gestión de cada entidad.', foto: 'SistematizacionLeccionesAprendidas.png' }
      ]
    }
  }
}
</script>

<style  scoped>

  .container-config{
    width: 70%;
    margin-bottom: 20px;
  }
/* @media screen and (min-width: 1440px) {
  .container-config{
      max-width: 50% !important;
  }
} */
  .shoit-dec{
    font-family: 'Raleway';
    font-style: normal;
    font-weight: 400;
    font-size: 20px !important;
    line-height: 19px;
    display: flex;
    align-items: center;
    text-align: center;
    color: #000000;
  }
  .ancho{
    margin: auto;
    margin-left: 120px;
    width: 90%;
    align-content: stretch;
  }
  .about-us{
    background-color: rgba(217, 215, 255, 0.6);;
  }
  .about-title{
    margin: 40px 0;
    margin-bottom: 50px;
    background-color: #fff;
  }
  .about-title p {

    font-family: 'Raleway';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 19px;
    display: flex;
    align-items: center;
    text-align: center;
  }
  .about-title img, .about-title video{
    margin-top: 20px;
  }
  .metodology-card{
    background-color: white;
    height: max-content;
    max-width: 340px;
    margin: 5px;
    padding: none;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  }
</style>
