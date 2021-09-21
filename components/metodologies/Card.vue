<template>
    <div>
        <h3 class="mb-3">{{title}}</h3>
        <p>{{description}} </p>
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
    title: {
      type: String,
      default: 'Amet minim mollit'
    }
  }
}
</script>
