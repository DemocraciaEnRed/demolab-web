<template>
  <div class="">
    <div id="challenges">
      <div class="secondary-bkg">
        <div class="container mx-6 stats-title columns">
          <div class="column is-two-fifths">
            <h3>Retos</h3>
            <h3>de ciudad</h3>
          </div>
          <div class="column ml-6">
            <p class="has-text-right parraf">
              Los retos de ciudad son los procesos que el Concejo de Bogotá
              <br />abre a la participación de la ciudadanía de Bogotá. Podrás
              proponer,<br />
              debatir con otras personas, votar y ser parte de las decisiones de
              la <br />ciudad.
            </p>
          </div>

          <!-- <span class="material-icons">
            double_arrow
          </span> -->
        </div>
      </div>
      <div class="container section columns">
        <div class="column box">
          <img src="~/assets/pot.png" alt="">
          <h3>la ruta pot</h3>
        </div>
        <div class="column box">
          <img src="~/assets/dialogok.png" alt="">
          <h3>la ruta pot</h3>
        </div>
        <div class="column box">
          <img src="~/assets/manifesta.png" alt="">
          <h3>la ruta pot</h3>
        </div>
        <div class="column box">
         <img src="~/assets/agenda-ciudadana.png" alt="">
          <h3>la ruta pot</h3>
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
export default {
  name: 'Stats'
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
  display: flex;
  align-items: center;
  padding: 10px;
}
.stats-title .material-icons {
  margin-left: 30px;
}
#challenges {
  background: #d9d7ff;
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

.box {
  border: solid 1px black;
  width: 265px;
  height: 265px;
  margin: 10px;
}
@media only screen and (max-width: 768px) {
  .stats {
    top: 0;
  }
  .stats-title {
    display: flex;
    justify-content: center;
  }
  .chall h2 {
    font-size: 44px;
    line-height: 36px;
  }
}
</style>
