<template>
  <div class="link" :style="{ backgroundColor: color }">
    <h3>{{ title }}</h3>
    <div class="link-content">
      IR
      <span class="material-icons">
        double_arrow
      </span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Link',
  props: {
    title: {
      type: String,
      default: ''
    },
    color: {
      type: String,
      default: '#333'
    }
  }
}
</script>

<style>
.link{
  font-family: "Staatliches", Helvetica, Arial, sans-serif;
  display: flex;
  width: 25%;
  padding: 10px;
  align-items: center;
  padding: 10px 0;
  justify-content: center;
}
.link h3{
  white-space: pre;
  margin-right: 25px;
  text-transform: uppercase;
  font-size: 20px;
  line-height: 25px;
}
.link-content{
  display: flex;
  font-size: 20px;
  align-items: center;
}
@media only screen and (max-width: 768px) {
  .link-content{
    position: absolute;
    right: 20px;
  }
}
</style>
