<script setup>
import fotografo from "../assets/fotografo (1).png";
</script>

<template>

<section class="banner">
<div>
<h1>
    Onde a paisagem vira 
    <span>Inspiração.</span>
</h1>
<p>Explore paisagens, cores e luzes que inspiram novas histórias através da fotografia.</p>
</div>
<img :src="fotografo" alt="Fotógrafo com câmera">
</section>

</template>

<style scoped lang="scss">
.banner {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 2rem;
  gap: 2rem;

  div {
    width: 50%;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  h1 {
    font-size: 2.8rem;
    line-height: 1.1;
  }

  span {
    color: #E1306C;
    font-size: 4.5rem;
  }

  img {
    width: 45%;
    max-width: 450px;
  }

  
  @media (max-width: 992px) {
    h1 {
      font-size: 2.4rem;
    }

    span {
      font-size: 3.5rem;
    }

    img {
      width: 40%;
      max-width: 380px;
    }

    div {
      width: 55%;
    }
  }

  
  @media (max-width: 576px) {
    flex-direction: column-reverse;
    text-align: center;

    div {
      width: 100%;
    }

    img {
      width: 80%;
      max-width: 280px;
    }

    h1 {
      font-size: 2rem;
    }

    span {
      font-size: 2.6rem;
    }

    p {
      font-size: 1rem;
      margin-top: 0.6rem;
    }
  }
}
</style>
