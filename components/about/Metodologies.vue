<template>
  <div class="container methodologies">
    <h1>Metodologias</h1>
    <div class="list">
      <div class="method">
        <h3>Metodologia #1</h3>
        <div />
      </div>
      <div class="method">
        <h3>Metodologia #2</h3>
        <div />
      </div>
      <div class="method">
        <h3>Metodologia #3</h3>
        <div />
      </div>
      <div class="method">
        <h3>Metodologia #4</h3>
        <div />
      </div>
      <div class="method">
        <h3>Metodologia #5</h3>
        <div />
      </div>
      <div class="method">
        <h3>Metodologia #6</h3>
        <div />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Metodologies'
}
</script>

<style scoped>
  .methodologies{
    padding: 20px 0;
    position: relative;
    top: 35px;
  }
  .list{
    display: flex;
    justify-content: space-between;
  }
  .method{
    margin: 0 10px;
    text-align: center;
  }
  .method div{
    height: 100px;
    border: 1px solid #D6D6D6;
    background-color: white;
    width: 175px;
  }
</style>
