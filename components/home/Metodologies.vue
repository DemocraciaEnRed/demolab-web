<template>
  <div class="methods-container">
    <div class="container methods">
      <div class="method-list">
        <div class="method">
          Metodologia 1
          <img src="https://via.placeholder.com/150" alt="">
        </div>
        <div class="method">
          Metodologia 2
          <img src="https://via.placeholder.com/150" alt="">
        </div>
        <div class="method">
          Metodologia 3
          <img src="https://via.placeholder.com/150" alt="">
        </div>
      </div>
      <div class="method-description">
        <h1>Metodologías</h1>
        <p>Conoce, descarga y aplica las metodologías de apertura de DemoLab</p>
        <Button :text="'ir a metodologias'" />
      </div>
    </div>
    <div class="link-container">
      <div class="container">
        <h1>Enlaces</h1>
      </div>
      <div class="links">
        <Link :title="'¿Que es el \n consejo de bogotá?'" :color="'rgba(92, 73, 186, 0.45)'" />
        <Link :title="'Agenda del Concejo'" :color="'rgba(0, 213, 189, 0.35)'" />
        <Link :title="'Proyectos de innovación \n política en el mundo'" :color="'rgba(217, 215, 255, 0.8)'" />
        <Link :title="'Data sets'" :color="'rgba(118, 219, 122, 0.57)'" />
      </div>
    </div>
  </div>
</template>

<script>
import Link from './Link.vue'

export default {
  name: 'Metodologies',
  components: {
    Link
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
  }
  .method-description{
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
    margin: 10px;
  }
  .methods{
    display: flex;
  }
  .links{
    display: flex;
    color: black;
  }
</style>
