<template>
  <div class="">
    <div id="challenges">
      <div class="secondary-bkg">
        <div class=" pt-6 mx-6 stats-title">
          <div class="  columns is-desktop">
            <div class="column">
              <h3 class="has-text-white">Retos</h3>
              <h3>de ciudad</h3>
              <!-- <div class="pt-4">
                <Button :transparent="true" :urlLink="'https://participa.demolab.com.co/'"/>
              </div> -->
            </div>
            <div class="column">
              <p class="parraf">
                Los retos de ciudad son los procesos que el Concejo de Bogotá
                abre a la participación de la ciudadanía de Bogotá. Podrás
                proponer,
                debatir con otras personas, votar y ser parte de las decisiones de
                la ciudad.
              </p>
            </div>
          </div>
        </div>
      </div>
      <div class="line container section is-justify-content-center is-flex-wrap-nowrap is-align-content-center">
        <div class="container section is-flex-tablet">
          <div class="box is-flex is-flex-direction-column is-justify-content-center is-flex-wrap-nowrap is-align-content-center">
            <div class="is-align-content-center">
              <img src="~/assets/pot.png" alt="" class="image is-150x150">
            </div>
            <div class="text-box is-align-content-center">
              <h3>la ruta pot</h3>
            </div>
          </div>
          <div class="box">
            <div>
              <img src="~/assets/dialogok.png" alt="" class="image is-150x150 ml-6 pl-5 mt-3">
            </div>
            <div class="text-box pt-6 mt-1">
              <h3>la ruta pot</h3>
            </div>
          </div>
          <div class="box">
            <div>
              <img src="~/assets/manifesta.png" alt="" class="image is-150x150 ml-6 pl-5 mt-3">
            </div>
            <div class="text-box pt-6 mt-3">
              <h3>la ruta pot</h3>
            </div>
          </div>
          <div class="box">
            <div>
              <img src="~/assets/agenda-ciudadana.png" alt="" class="image is-150x150 ml-6 pl-5">
            </div>
          <div class="text-box pt-5">
              <h3>la ruta pot</h3>
          </div>
          </div>
        </div>
      </div>

      <!-- <div class="first-challenge column chall">
        <h2 class="feature-number">
          2
        </h2>
        <h3>Retos <br> publicados</h3>
      </div>
      <div class="column chall">
        <img src="/images/stats-ideas.png" alt="">
        <div>
          <h2 class="feature-number">
            20
          </h2>
          <h3>Consultas</h3>
        </div>
      </div>
      <div class="column chall">
        <img src="/images/stats-opinion.png" alt="">
        <div>
          <h2 class="feature-number">
            1000
          </h2>
          <h3>participantes</h3>
        </div>
      </div>
      <div class="column chall">
        <img src="/images/stats-comments.png" alt="">
        <div>
          <h2 class="feature-number">
            5000
          </h2>
          <h3>comentarios</h3>
        </div>
      </div> -->
    </div>
  </div>
</template>

<script>
// import Button from '@/components/Button.vue'

export default {
  name: 'Stats',
  components: {
  }
}
</script>

<style>
.parraf {
  font-family: Raleway;
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 23px;
  text-align: right;
  color: #ffffff;
}
.chall {
  display: flex;
  justify-content: center;
}
.chall h2 {
  font-size: 25px;
  line-height: 11px;
}
.chall div {
  margin-left: 5px;
  align-self: center;
}
.feature-number {
  color: #5c49ba;
}
.stats-title h3 {
  line-height: 40px;
  font-size: 40px;
  color: #5fd1bc;
}
.stats-title h4 {
  font-size: 30px;
  line-height: 30px;
  color: white;
}
.stats {
  position: relative;
  top: -30px;
}
.stats-title {
  color: white;
  height: 141px;
  /* display: flex; */
  align-items: center;
  padding: 10px;
}
.stats-title .material-icons {
  margin-left: 30px;
}
#challenges {
  background: #5c49ba;
  align-items: center;
}
.first-challenge {
  display: flex;
  align-items: center;
}
.first-challenge h2 {
  font-size: 80px;
}
.first-challenge h3 {
  font-size: 30px;
  line-height: 30px;
  vertical-align: middle;
}
hr{
  margin: 0;
  height:200px;
  background-color:red;
  z-index: 0;
  position: relative;
}
.line{
  display: flex;
  background-color: #584DB3;
  height: 150px;
  margin-bottom: 250px;
  margin-left: 3rem;
}
.box {
  z-index: 1000;
  width: 265px;
  height: 265px;
  margin: 10px;
  justify-content: center;
  border-bottom: 5px solid rgba(98, 102, 105, 0.19);
  /* -webkit-box-shadow: 0px 5px 12px -1px rgba(0,0,0,0.85);
  box-shadow: 0px 5px 12px -1px rgba(0,0,0,0.85); */
}
.text-box{

  font-family: Staatliches;
  font-style: normal;
  font-weight: normal;
  font-size: 25px;
  line-height: 31px;
  text-align: center;

  color: #584DB3;
}
img .image{
  margin: auto;
}
@media only screen and (max-width: 768px) {
  .line{
    height: auto;
    margin-bottom: 10px;
    margin-left: 0px;
  }
  .stats {
    top: 0;
  }
  .stats-title {
    display: flex;
    justify-content: center;
    height: auto;
  }
  .chall h2 {
    font-size: 44px;
    line-height: 36px;
  }
  .parraf{
    text-align: left;
    padding: 0px;
  }
}
@media only screen and (min-width: 1366px) {
  .line {
    margin-left:8rem !important;
  }

}
</style>
