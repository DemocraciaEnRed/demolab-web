<template>
  <a class="boton" :class="{ full: fullwidth, secondary: secondary, primary: primary}">
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
    text: {
      type: String,
      default: 'Ver más'
    },
    icon: {
      type: String,
      default: 'double_arrow'
    }
  }
}
</script>

<style>

</style>
