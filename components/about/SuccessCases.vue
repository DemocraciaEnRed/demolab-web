<template>
  <div class="success">
    <div class="container">
      <h1>Casos de exito</h1>
      <div class="columns">
        <div class="column success-card" />
        <div class="column success-card" />
        <div class="column success-card" />
        <div class="column success-card" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SuccessCases'
}
</script>

<style>
.success{
  margin: 50px 0;
  background-color: #FAFAFA;
}
.success h1{
  font-size: 40px;
  text-align: left;
}
.success-card{
  background-color: white;
  height: 150px;
  margin: 5px;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}
</style>
