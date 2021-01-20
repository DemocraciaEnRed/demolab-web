<template>
  <div class="container stats">
    <div id="challenges">
      <div class="stats-title secondary-bkg column">
        <div>
          <h4>Retos</h4>
          <h3>de ciudad</h3>
        </div>
        <span class="material-icons">
          double_arrow
        </span>
      </div>
      <div class="first-challenge column chall">
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
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Stats'
}
</script>

<style>
  .chall{
    display: flex;
    justify-content: center;
  }
  .chall h2{
    font-size: 25px;
    line-height: 11px;
  }
  .chall div{
    margin-left: 5px;
    align-self: center;
  }
  .feature-number{
    color: #5C49BA;
  }
  .stats-title h3{
    line-height: 40px;
    font-size: 40px;
    color: #5FD1BC;
  }
  .stats-title h4{
    font-size: 30px;
    line-height: 30px;
    color: white;
  }
  .stats{
    position: relative;
    top: -30px;
  }
  .stats-title{
    color: white;
    height: 141px;
    display: flex;
    align-items: center;
    padding: 10px;
  }
  .stats-title .material-icons{
    margin-left: 30px;
  }
  #challenges{
    background: #D9D7FF;
    align-items: center;
  }
  .first-challenge{
    display: flex;
    align-items: center;
  }
  .first-challenge h2{
    font-size: 80px;
  }
  .first-challenge h3{
    font-size: 30px;
    line-height: 30px;
    vertical-align: middle;
  }
  @media only screen and (max-width: 768px) {
    .stats{
      top: 0;
    }
    .stats-title{
      display: flex;
      justify-content: center;
    }
    .chall h2{
      font-size: 44px;
      line-height: 36px;
    }
  }
</style>
