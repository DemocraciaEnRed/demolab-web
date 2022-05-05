<template>
  <div>
    <footer>
      <div class="container is-justify-content-center">
        <div class="">
          <img src="/images/footer-logos.png" alt="logos de demo lab y de el consejo de bogota">
        </div>
        <!-- <ul class="sitemap">
          <li>¿Como funciona?</li>
          <li>Acerca de este sitio</li>
          <li>Contacto</li>
        </ul>
        <ul class="terms">
          <li>Terminos y condiciones</li>
          <li>Politica de privacidad</li>
        </ul> -->
      </div>
    </footer>
    <div class="sponsors">
      <h5 class="has-text-centered">
        Con el apoyo de
      </h5>
      <div id="sponsors" class="columns is-desktop">
        <div class="column is-one-quarter is-flex">
          <img class="image" src="/images/sponsor-corona.png" alt="Fundación corona">
          <img class="image"  src="/images/sponsor-avina.png" alt="Fundación avina">
        </div>
        <div class="column is-one-quarter is-flex">
          <img class="image" src="/images/sponsor-FESCOL.png" alt="Fescol" >
          <img class="image" src="/images/sponsor-extituto.png" alt="Extituto, politica abierta">
        </div>
        <div class="column is-one-quarter is-flex">
          <img class="image" src="/images/sponsor-idemos.png" alt="ideemos, laboratorio de innovación democratica">
          <img class="image" src="/images/sponsor-NIMD.png" alt="netherlands institute for multiparty democracy">
        </div>
        <div class="column is-one-quarter is-flex-desktop is-justify-content-center">
          <img class="image" src="/images/sponsor-diseno-publico.png" alt="diseño público">
        </div>
      </div>
      <!-- <ul class="container sponsor-list columns is-mobile">
        <li class="column is-one-third-mobile">
          <img class="image" src="/images/sponsor-corona.png" alt="Fundación corona">
        </li>
        <li class="column">
          <img class="image"  src="/images/sponsor-avina.png" alt="Fundación avina">
        </li>
        <li class="column">
          <img class="image" src="/images/sponsor-FESCOL.png" alt="Fescol">
        </li>
        <li class="column">
          <img class="image" src="/images/sponsor-extituto.png" alt="Extituto, politica abierta">
        </li>
        <li class="column">
          <img class="image" src="/images/sponsor-idemos.png" alt="ideemos, laboratorio de innovación democratica">
        </li>
        <li class="column">
          <img class="image" src="/images/sponsor-NIMD.png" alt="netherlands institute for multiparty democracy">
        </li>
        <li class="column">
          <img class="image" src="/images/sponsor-diseno-publico.png" alt="diseño público">
        </li>
      </ul> -->
    </div>
    <div class="secondary-bkg">
      <div class="container">
        <div class="democracy-os">
          <div>
            <img src="/images/icon-democracy-os.png" alt="logo de democracia en red">
            <span>Desarrollado con ❤️ <br>por <strong>Democracia en Red</strong></span>
          </div>
          <p class="rights">
            Todos los derechos reservados
          </p>
          <div class="has-text-white">
            <a href="https://twitter.com/DemoLabCA" target="_blank">
              <span class="fa fa-2x fa-twitter mx-6" style="color:#fff"></span>
            </a>
            <a href="https://www.facebook.com/demolabca/" target="_blank">
              <span class="fa fa-2x fa-facebook mx-6" style="color:#fff"></span>
            </a>
            <a href="https://www.instagram.com/demolabca/?hl=es" target="_blank">
              <span class="fa fa-2x fa-instagram mx-6" style="color:#fff"></span>
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style>
  .dummy{
    width: 200px;
  }
  .sponsor-list{
    text-align: center;
    margin: auto;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .sponsor-list li{
    margin: 0 5px;
  }
  footer>div{
    display: flex;
    align-items: center;
    padding: 20px 0;
  }
  footer{
    background-color: #F5F5F5;
  }
  .terms{
    margin-left: auto;
  }
#sponsors div img{
  max-height:118px;
  margin: auto;
}
  .sponsors{
    background-color: #E8E8E8;
  }
  .sponsors h5{
    padding: 10px 0;
    font-family: 'Raleway', sans-serif;
    font-weight: bold;
    text-transform: uppercase;
  }
  .democracy-os img{
    width: 31px;
    height: 26.57px;
  }
  .rights{
    align-self: center;
  }
  .democracy-os strong{
    color: white;
  }
  .democracy-os div{
    display: flex;
    padding: 10px 0;
  }
  .democracy-os{
    color: white;
    display: flex;
    justify-content: space-between;
  }
  .sitemap, .terms{
    font-family: "Staatliches", Helvetica, Arial, sans-serif;
    color: #584DB3;
  }
  .sitemap{
    margin-left: 20px;
  }
  .terms{
    color: #333;
  }
  @media only screen and (max-width: 768px) {
    footer{
      padding: 0px 20px;
    }
    .logos-footer{
      max-width: 50px;
    }
    .democracy-os{
      flex-direction: column;
    }
    .democracy-os div{
      justify-content: center;
    }
  #sponsors{
    height: auto;
    justify-content: center;
  }
  #sponsors div img {
    padding: 30px 0px !important;
  }
  }
</style>
