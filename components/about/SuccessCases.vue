<template>
  <div class="success">
    <div class="container">
      <h1 class="my-6 has-text-centered-mobile">Casos de exito</h1>
      <p class="m-2 py-3">
        <span class="indicator is-hidden-desktop is-size-3">desliza la tarjeta >>> </span>
      </p>
       <b-carousel-list
            :data="items"
            :arrow="arrow"
            :arrow-hover="arrowHover"
            :items-to-show="perList"
            :items-to-list="increment"
            :repeat="repeat"
            :has-drag="drag"
            :has-grayscale="gray"
            :has-opacity="opacity"
            >
                <template #item="list" :id="`card-template`"  style="width:0px !important;">
                   <div :id="`${list.title}`" class="sucess-case">
                      <!-- <h3 class="case-title text-center" :style="{ color: color }"> -->
                      <h3 class="case-title text-center" >
                        {{ list.title }}
                      </h3>
                      <p class="case-description py-3">
                        {{ list.descripcion }}
                      </p>
                    </div>
                </template>
       </b-carousel-list>
      <!-- modelo viejo -->
      <!-- <b-carousel
        progress
        progress-type="is-primary"
        :auto-play="false"
        :items-to-show="perList"
        :items-to-list="increment"
        :repeat="repeat"
        :has-drag="drag"
      >
        <b-carousel-item v-for="(item, i) in items" :key="i" class="p-6">
          <section class="column is-flex is-justify-content-center">
            <SucessCaseCard
              id=i
              :color="'#000000'"
              :title="`${item.title}`"
              :description="`${item.descripcion}`"
            />
          </section>
        </b-carousel-item>
      </b-carousel> -->
    </div>
  </div>
</template>

<script>
// import SucessCaseCard from './SucessCaseCard.vue'
// const cardList = this.document.querySelectorAll('carusel-slide')
// console.log(cardList)
export default {
  name: 'SuccessCases',
  components: {
    // SucessCaseCard
  },
  mounted () {
    const resolution = window.screen.width
    if (resolution > 720) {
      this.perList = 2.5
    } else {
      this.perList = 1
    }
  },
  data () {
    return {
      arrow: false,
      arrowHover: true,
      drag: true,
      gray: false,
      opacity: false,
      values: 1,
      perList: 3,
      increment: 1,
      repeat: false,
      items: [
        { title: 'Reconocimiento OCDE', descripcion: 'En 2021 la Organización de Cooperación y Desarrollo Económico OCDE, resaltó el modelo de Asamblea Ciudadana Itinerante realizada por el Concejo de Bogotá y diseñada e implementada por el DemoLab, como un caso de éxito en el fortalecimiento de la democracia deliberativa y éste, fue el único a nivel de una corporación público administrativa y el único en América Latina' },
        { title: 'Reconocimiento Universidad Externado', descripcion: 'En 2021 La Universidad Externado de Colombia presentó un dossier sobre innovación pública e innovación social y la estrategia de participación diseñada e implementada por el DemoLab,  Concejo a la Casa fue tomada como el primer caso de demoracia por aleatoriedad en Colombia.' },
        { title: 'Alianza con Enfoque de Género', descripcion: 'En 2021 se realizó el lanzamiento de la Caja de Herramientas para incorporar el enfoque de género en el trabajo que desarrolla el Concejo de la ciudad. Esta Caja fue diseñada por el DemoLab y en colaboración con coordinadores de las bancadas temáticas en temas de equidad y mujer del Concejo de Bogotá, la Secretaría de la Mujer y delegadas de ONU Mujeres, NIMD y Extituto de Política Abierta.' },
        { title: 'Cabildos Abiertos ante la crisis social', descripcion: 'En 2021, La metodología de Concejo a la Calle fue diseñada para las sesiones abiertas del Concejo de Bogotá en la Plaza de Bolívary el Portal de las Américas. A través de DemoLab, se canalizaron  diversas expresiones ciudadanas y el análisis recogido de la participació de las y los habitantes se logró presentar en un informe de resultados dirigido al gobierno nacional' }
      ]
    }
  }
}
</script>

<style lang="scss" scope>

.success {
  margin: 50px 0;
  background-color: #fafafa;
}
.success h1 {
  font-size: 40px;
  text-align: left;
}
.success-card {
  background-color: white;
  height: max-content;
  margin: 5px;
  margin-bottom: 15px;
  border-left: solid 20px #5c49ba;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}
 .carusel-item{
  width:0px !important;
}
 .sucess-case{
    height: 270px ;
    position: relative;
    padding: 20px;
    border-left: 20px solid #5C49BA;
    width: 519px;
    background: #FFFFFF;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
    margin: 0px !important;
  }
  .event{
    background-color: white;
    margin: 0px 5px;
  }

  .case-title {
    margin-right: 15px;

    font-family: Staatliches;
    font-style: normal;
    font-weight: normal;
    font-size: 25px;
    line-height: 31px;

    color: #000000;

  }
  .case-description, .event-title{

    font-family: Raleway;
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 19px;
    padding-top: 20px;
    color: #090909;

  }
  .event-description{
    text-align: center;
  }

.indicator{
  color:#8e86b696;
}

  @media screen and (max-width: 740px) {
    .sucess-case{
      min-height: 100%;
      height: auto;
      position: relative;
      padding: 20px;
      border-left: 20px solid #5C49BA;
      width: auto;
      background: #FFFFFF;
      box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
      margin: 0px !important;
  }
  }
</style>
