<template>
  <div class="container about-us">
    <div class="has-text-centered about-title">
      <h3>Sobre nosotros</h3>
      <h1>¿Que es demolab?</h1>
      <p>Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint. <br> Velit officia consequat duis enim velit mollit. Exercitation veniam consequat sunt nostrud amet.</p>
       <iframe
          src="https://player.vimeo.com/video/446827718"
          width="640"
          height="360"
          frameborder="0"
        />
    </div>
    <div class="features-about">
      <div class="columns">
        <div class="column text is-left">
          <h1>¿Qué es, para qué es y cómo funciona el DemoLab?</h1>
          <p>Aliqua id fugiat nostrud irure ex duis ea quis id quis ad et. Sunt qui esse pariatur duis deserunt mollit dolore cillum minim tempor enim. Elit aute irure tempor cupidatat incididunt sint deserunt ut voluptate aute id deserunt nisi.</p>
        </div>
        <div class="column text is-right">
          <img src="https://via.placeholder.com/150" alt="">
        </div>
      </div>
      <div class="columns reverse-mobile">
        <div class="column text  is-left">
          <img src="https://via.placeholder.com/150" alt="">
        </div>
        <div class="column text  is-right">
          <h1>¿Qué es, para qué es y cómo funciona el DemoLab?</h1>
          <p>Aliqua id fugiat nostrud irure ex duis ea quis id quis ad et. Sunt qui esse pariatur duis deserunt mollit dolore cillum minim tempor enim. Elit aute irure tempor cupidatat incididunt sint deserunt ut voluptate aute id deserunt nisi.</p>
        </div>
      </div>
      <div class="columns">
        <div class="column text">
          <h1>¿Qué es, para qué es y cómo funciona el DemoLab?</h1>
          <p>Aliqua id fugiat nostrud irure ex duis ea quis id quis ad et. Sunt qui esse pariatur duis deserunt mollit dolore cillum minim tempor enim. Elit aute irure tempor cupidatat incididunt sint deserunt ut voluptate aute id deserunt nisi.</p>
        </div>
        <div class="column text is-right">
          <img src="https://via.placeholder.com/150" alt="">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AboutHeader'
}
</script>

<style>
.about-title{
  margin: 40px 0;
  margin-bottom: 60px;
}
.about-title iframe{
  width: 100%;
  max-width: 650px;
  margin-top: 20px;
}
.features-about{
  padding: 0 10px;
}
.features-about .columns{
  margin: 40px 0;
}
.features-about h1{
  line-height: 40px;
}
.is-right{
  text-align: right;
}
.is-left{
  text-align: left;
}
@media only screen and (max-width: 768px) {
  .text{
    text-align: center;
  }
  .reverse-mobile{
    flex-direction: column-reverse;
    display: flex;
  }
}
</style>
