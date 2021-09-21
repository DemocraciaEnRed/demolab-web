<template>
    <div>
        <img src="https://via.placeholder.com/450x250" alt="">
        <p>{{description}} </p>
        <p v-if="readMore">{{moreDescription}} </p>
        <button @click="showMore" v-if="!readMore" class="boton"><span class="mateirla-icons">Leer más</span></button>
        <button @click="showLess" v-if="readMore" class="boton"><span class="mateirla-icons">Leer Menos</span></button>
    </div>
</template>

<script>

export default {
  name: 'ServicesSuccessCase',
  props: {
    description: {
      type: String,
      default: 'Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint.'
    },
    moreDescription: {
      type: String,
      default: 'Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint.'
    }
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
