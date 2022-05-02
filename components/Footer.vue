<template>
  <div>
    <footer>
      <div class="container">
        <div class="logos-footer">
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
      <ul class="container sponsor-list">
        <li>
          <img src="/images/sponsor-corona.png" alt="Fundación corona">
        </li>
        <li>
          <img src="/images/sponsor-avina.png" alt="Fundación avina">
        </li>
        <li>
          <img src="/images/sponsor-FESCOL.png" alt="Fescol">
        </li>
        <li>
          <img src="/images/sponsor-extituto.png" alt="Extituto, politica abierta">
        </li>
        <li>
          <img src="/images/sponsor-idemos.png" alt="ideemos, laboratorio de innovación democratica">
        </li>
        <li>
          <img src="/images/sponsor-NIMD.png" alt="netherlands institute for multiparty democracy">
        </li>
        <li>
          <img src="/images/sponsor-diseno-publico.png" alt="diseño público">
        </li>
      </ul>
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
  }
</style>
