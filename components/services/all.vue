<template>
    <div>
        <div class="container">
            <h1 class="has-text-centered">Servicios</h1>
        </div>
        <div class="section">
            <div class="container card-list">
        <div class="tile is-ancestor is-flex is-justify-content-center">
          <div class="card card-config mx-6">
            <div class="card-image">
              <img src="~/assets/participacion_mano.png" alt="imagen participacion e incidencia">
            </div>
            <div class="title is-4 has-text-centered mt-3">Línea de participación y apertura del Concejo</div>
            <div class="card-content content">Diseñamos y desarrollamos herramientas, proyectos, actividades, tecnología cívica y habilitación de la incidencia ciudadana en los procesos de toma de decisión del Concejo de Bogotá</div>
          </div>
          <div class="card card-config mx-6">
            <div class="card-image">
              <img src="~/assets/participacion_rayo.png" alt="aceleracio na la innovacion">
            </div>
            <div class="title is-4 has-text-centered mt-3">Línea de aceleración a la innovación en el Concejo</div>
            <div class="card-content content">Creamos metodologías de  innovación pública, desarrollo de prototipos, diseño público, habilitación, acompañamiento y fortalecimiento de la innovación en el Concejo de Bogotá</div>
          </div>
          <div class="card card-config mx-6">
            <div class="card-image">
              <img src="~/assets/gestion_foco.png" alt="gestion del conocimiento">
            </div>
            <div class="title is-4 has-text-centered mt-3">Línea de Gestión del conocimiento</div>
            <div class="card-content content">Construimos una red de acción e investigación con la academia, organizaciones de la sociedad civil, semilleros y el ecosistema de innovación pública, para el fortalecer la gestión del conocimiento al interior de la Corporación</div>
          </div>
        </div>
            </div>
        </div>
        <div class="section">
            <h1 class="has-text-centered">cifras de experiencias exitosas</h1>
            <div class="container is-flex is-flex-wrap-wrap is-justify-content-center">
                <img src="~assets/servicios/LaRutaPOT.png" alt="">
                <img src="~assets/servicios/Toolkit.png" alt="">
                <img src="~assets/servicios/Habilitacion.png" alt="">
                <img src="~assets/servicios/Conocimiento.png" alt="">
            </div>
        </div>
    </div>
</template>
<script>

export default {
  name: 'allPage',
  components: {
  }
}
</script>

<style scoped>
    .events{
    display: flex;
    flex-direction: row;
    }
    .card-list{
        display: flex;
        flex-direction: row;
        align-items: center;
        align-content: space-between;
        margin-left: 5px;
    }
    .card-config{
        max-width: 220px;
    }
</style>
