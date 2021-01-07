<template>
  <div class="bogota">
    <div class="participate">
      <div class="participate-main">
        <img
          class="logo-participate"
          src="/images/logo.png"
          alt="Demo lab, concejo abierto"
        >
        <p>
          Participa en los procesos de toma de decisión del Concejo de Bogotá para construir entre todos y todas una mejor ciudad
        </p>
      </div>
      <div class="participate-features">
        <div class="p-feature-grup">
          <div>
            <img src="/images/feat-ciudadania.png" alt="ilustracion de manos alzadas">
            <span>Propone</span>
          </div>
          <div>
            <img src="/images/feat-voto.png" alt="ilustracion de persona votando">
            <span>Vota</span>
          </div>
          <div>
            <img src="/images/feat-agenda.png" alt="ilustracion de agenda">
            <span>Prioriza</span>
          </div>
        </div>
        <Button :text="'Participa e incide'" :secondary="true" />
      </div>
    </div>
  </div>
</template>

<script>
import Button from '../Button.vue'

export default {
  name: 'Participate',
  components: { Button }
}
</script>

<style>
  .bogota{
    background-image: url('/images/bogota.png');
    padding: 50px 0;
  }
  .participate{
    background-color: white;
    width: 60%;
    display: flex;
  }
  .logo-participate{
    width: 200px;
  }
  .p-feature-grup{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }
  .participate .boton{
    position: relative;
    right: -80px;
  }
  .participate-main{
    position: relative;
    top: -30px;
    padding: 15px;
    margin-left: 50px;
  }

</style>
