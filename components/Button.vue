<template>
  <a class="boton" :href="urlLink" :class="{ full: fullwidth, secondary: secondary, primary: primary, transparent: transparent}" :style="`background-color:${ccolor}`">
    {{ text }}
    <span class="material-icons">
      {{ icon }}
    </span>
  </a>
</template>

<script>
export default {
  name: 'Button',
  props: {
    urlLink: {
      type: String,
      default: '.'
    },
    fullwidth: {
      type: Boolean,
      default: false
    },
    secondary: {
      type: Boolean,
      default: false
    },
    primary: {
      type: Boolean,
      default: false
    },
    transparent: {
      type: Boolean,
      default: false
    },
    text: {
      type: String,
      default: 'Ver más'
    },
    icon: {
      type: String,
      default: 'double_arrow'
    },
    ccolor: {
      type: String,
      default: '#5C49BA'
    }
  }
}
</script>

<style>
.boton{
  background-color: #5C49BA;
  font-weight: normal !important;
}
</style>
