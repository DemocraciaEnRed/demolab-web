<template>
  <div class=" columns bogota">
    <div class="column is-one-third participate">
      <div class="participate-main">
        <img
          class="logo-participate"
          src="/images/logo.png"
          alt="Demo lab, concejo abierto"
        >
        <p class="has-background-bl parrafo">
          Participa en los procesos de toma de decisión del Concejo de Bogotá para construir entre todos y todas una mejor ciudad
        </p>
      <div class="participate-features">
        <!-- <div class="p-feature-grup">
          <table>
            <tr class="feature-images">
              <td>
                <img src="/images/feat-ciudadania.png" alt="ilustracion de manos alzadas">
              </td>
              <td>
                <img src="/images/feat-voto.png" alt="ilustracion de persona votando">
              </td>
              <td>
                <img src="/images/feat-agenda.png" alt="ilustracion de agenda">
              </td>
            </tr>
            <tr>
              <td>
                <h2 class="secondary-color">
                  Propone
                </h2>
              </td>
              <td>
                <h2 class="secondary-color">
                  Vota
                </h2>
              </td>
              <td>
                <h2 class="secondary-color">
                  Prioriza
                </h2>
              </td>
            </tr>
          </table>
        </div> -->
        <Button :href="'https://participa.demolab.com.co/'" :text="'Participa e incide'" :secondary="true" />
      </div>
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
    width: 60%;
    display: flex;
  }
  .logo-participate{
    width: 200px;
  }
  .participate-features{
    margin-top: 20px;
    display: inline-block;
    flex-direction: row;
    /* justify-content: center; */
  }
  .participate .boton{
    /* position: relative;
    right: -80px; */
  }
  .feature-images img{
    width: 94px;
  }
  .parrafo{
    font-family: Raleway;
    font-style: normal;
    font-weight: 600;
    font-size: 18px;
    line-height: 16px;
    display: flex;
    align-items: center;
    color: #000000;
  }
  .feature-images td{
    vertical-align: bottom;
  }
  .p-feature-grup table{
    text-align: center;
    width: 100%;
  }
  .p-feature-grup table{
    width: 100%;
  }
  .participate-main{
    position: relative;
    top: -30px;
    padding: 15px;
    margin-left: 50px;
  }
  @media only screen and (max-width: 768px) {
    .participate{
      width: 100%;
      flex-direction: column;
      margin-bottom: 10px;
    }
    .participate-main{
      text-align: center;
      margin: 0;
    }
    .participate-features .boton{
      right: 0;
    }
    .bogota{
      padding: 10px;
    }
  }
</style>
