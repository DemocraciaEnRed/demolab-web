<template>
  <div class="methods-container">
    <div class="container methods">
      <div class="method-list">
        <div id="rutapot" class="method">
          #LARUTAPOT
          <img src="~assets/RutaPOT 1.png" alt="">
        </div>
        <div class="method is-size-6-mobile">
          Cultura de la Innovación
          <img src="~assets/ToolkitGenero 1.png" alt="">
        </div>
        <div class="method is-size-5-mobile">
          tOOLKIT DE gENERO
          <img src="~assets/CulturaInnovacion 1.png" alt="">
        </div>
      </div>
      <div class="method-description">
        <h1>Proyectos</h1>
        <p>Generamos espacios de participación incidente y mecanismos innovadores para responder a los retos distritales</p>
        <Button :transparent="true" :color="'$primary'" :text="'ir a proyectos'" :urlLink="'/metodologias'" />
      </div>
    </div>
    <!-- <div class="link-container">
      <div class="container">
        <h1>Enlaces</h1>
      </div>
      <div class="links">
        <Link :title="'¿Que es el \n consejo de bogotá?'" :color="'rgba(92, 73, 186, 0.45)'" />
        <Link :title="'Agenda del Concejo'" :color="'rgba(0, 213, 189, 0.35)'" />
        <Link :title="'Proyectos de innovación \n política en el mundo'" :color="'rgba(217, 215, 255, 0.8)'" />
        <Link :title="'Data sets'" :color="'rgba(118, 219, 122, 0.57)'" />
      </div>
    </div> -->
  </div>
</template>

<script>
// import Link from './Link.vue'

export default {
  name: 'Metodologies',
  components: {
    // Link
  }
}
</script>

<style scoped>
  .link-container h1{
    font-size: 40px;
    margin-top: 50px;
  }
  .methods-container{
    background: white;
    padding-top: 30px;
    margin-bottom: 80px;
    border-bottom: 2px solid $secondary;
  }
  .method-description{
    max-width: 390px;
    align-content: center;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    padding: 0 20px;
  }
  .method-list{
    display: flex;
  }
  .method{
    display: flex;
    flex-direction: column;
    margin: 0px 10px;
    font-family: 'Staatliches';
    font-style: normal;
    font-weight: 400;
    font-size: 20px;
    line-height: 25px;
    text-align: center;
    text-transform: uppercase;

    color: #3E3E3E;

  }
  .methods{
    display: flex;
  }
  .links{
    display: flex;
    color: black;
  }
  .method img{
    border: 2px solid #5C49BA;
  }
  @media only screen and (max-width: 768px) {
    .links{
      flex-direction: column;
    }
    .methods{
      flex-direction: column;
      width: 100%;
    }
    .method{
      margin: 0px 2px !important;
    }
    .method-description{
      text-align: center;
      align-items: center;
    }
    .link-container h1{
      text-align: center;
    }
    .link{
      width: 100%;
      justify-content: flex-start;
      padding: 10px 20px;
    }
    p{
      margin-bottom: 15px;
    }
  }

  @media only screen and (max-with: 420px) {

  }
</style>
