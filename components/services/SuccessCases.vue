<template>
  <div class="container mb-6">
    <h1>Experiencias Exitosas</h1>
    <div class="columns">
      <div class="column">
        <ServicesSuccessCase :description="'Una iniciativa que fortalece el debate sobre el Plan Distrital de Desarrollo en la corporación'" :moreDescription="''" />
      </div>
      <div class="column">
        <ServicesSuccessCase :description="'Es la primera Asamblea Ciudadana realizada por una corporación y logró reunir de manera virtual a ciudadanos y ciudadanas de Bogotá para deliberar sobre el Plan de ordenamiento Territorial.'" :moreDescription="''" />
      </div>
      <div class="column">
        <ServicesSuccessCase :description="'La ciudadanía priorizó la Política de Humedales presentada por la Bancada Colombia Patriótica en la sesion plenaria del 14 de diciembre de 2020'" :moreDescription="''" />
      </div>
      <div class="column">
        <ServicesSuccessCase :description="'Las organizaciones aliadas y el Laboratorio de Innovación Política del Concejo de Bogotá desarrolló una plataforma de participación e incidencia.'" :moreDescription="'En el marco de las alianzas estratégicas entre el Demolab y las organizaciones aliada como: el Extituto de Política Abierta, la Friedrich Ebert Stiftung y el Instituto Holandés para la Democracia Multipartidaria - NIMD y conjuntamente con DemocracyOS desarrollamos una plataforma de tecnología cívica para que tanto la ciudadanía como  a nivel interno (Concejales, Concejalas, equipos y funcionarios) logren vincular procesos de participación incidente.'" />
      </div>
    </div>
    <div class="columns">
      <div class="column">
        <ServicesSuccessCase :description="'En alianza con las organizaciones aliadas, prototipamos  una Caja de Herramientas para las y los Concejales y sus equipos, con el objetivo de fomentar la innovación pública.'" :moreDescription="'Este gran instrumento fue co creado con: el Extituto de Política Abierta, el ,El Instituto Holandés para la Democracia Multipartidaria (NIMD) la Secretaría Distrital de la Mujer y ONU Mujeres Colombia, con el involucramiento de la Bancada para la equidad de la Mujer, el sistema Distrital de Cuidado y Eliminación de todas las Violencias Basadas en Género , La Bancada de la Mujer. la Mesa Directiva de 2020 y 2021 del Concejo de Bogotá, hemos desarrollado una serie de herramientas que faciliten a Concejales, Concejalas y sus equipos, incorporar este enfoque dentro la labor normativa, de control político y presupuesto de ciudad..'" />
      </div>
      <div class="column">
        <ServicesSuccessCase :description="'En alianza con las organizaciones aliadas,  diseñamos y elaboramos una Caja de Herramientas para la transversalización del Enfoque de Género en el Concejo de Bogotá.'" :moreDescription="'Construimos un prototipo de una Caja de Herramientas con acceso directo a servicios, metodologías, y herramientas en formato digital, un kit de adhesivos para construir en un muro de las oficinas, un mapa sistémico que aborde temas relacionados a la gestión normativa de y control político. Acceso a los servicios del Laboratorio a través de un código QR que se encuentra ubicado en cada oficina, guia metodológica con las metodologías de servicio de habilitación y un documennto metodológico con efo'" />
      </div>
      <div class="column">
        <img src="https://via.placeholder.com/450x250" alt="">
        <p>Aliqua id fugiat nostrud irure ex duis ea quis id quis ad et</p>
        <button @click="showMore" v-if="!readMore" class="boton"><span class="mateirla-icons">Leer más</span></button>
        <button @click="showLess" v-if="readMore" class="boton"><span class="mateirla-icons">Leer Menos</span></button>
      </div>
    </div>
  </div>
</template>

<script>
import ServicesSuccessCase from './ServicesSuccessCase.vue'

export default {
  name: 'SuccessCases',
  components: {
    ServicesSuccessCase
  },
  data: () => ({
    readMore: false
  }),
  methods: {
    showMore () {
      this.readMore = true
    },
    showLess () {
      this.readMore = false
    }
  }
}
</script>

<style>

</style>
