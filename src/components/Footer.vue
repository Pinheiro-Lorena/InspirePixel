<script setup>
import Socialsicons from "../assets/Socials icons.png";
</script>

<template>
<footer> 
    
<div>
    <h3>Contato</h3>
    <ul>
        <li>contato@byinspiration.com</li>
        <li>Central de Ajuda</li>
        <li>São Paulo - Brasil 📍</li>
    </ul>
</div>

<div>
    <h3>Sobre</h3>
    <nav>
        <ul>
            <li>Politica de Privacidade</li>
            <li>Sobre Nós</li>
            <li>Blog</li>
        </ul>
    </nav>
</div>

<div>
    <h3>Redes Sociais</h3>
    <img :src="Socialsicons" alt="redes" />

</div>
                

<div>
    <h3>Assine nossa NewsLatter</h3>
 <input type="email">
 <button>Inscreva-se</button>

</div>
<p>© 2024 Inspire Pixel. Todos os direitos reservados.</p>
</footer>
</template>

<style scoped lang ="scss">
footer {
  width: 100%;
  background: #111;
  color: #f1f1f1;
  padding: 3rem 2rem;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  gap: 2.5rem;

  p {
    font-size: 0.95rem;
    opacity: 0.7;
    line-height: 1.4;
  }

  h3 {
    font-size: 1.1rem;
    margin-bottom: 1rem;
    font-weight: 600;
    color: #fff;
  }

  ul {
    list-style: none;
    padding: 0;

    li {
      margin-bottom: 0.5rem;
      font-size: 0.95rem;
      opacity: 0.8;
      cursor: pointer;
      transition: 0.3s;

      &:hover {
        opacity: 1;
      }
    }
  }

  input {
    width: 100%;
    padding: 0.7rem 1rem;
    border-radius: 6px;
    border: none;
    margin-bottom: 0.6rem;
    font-size: 0.95rem;
    outline: none;
  }

  button {
    width: 100%;
    padding: 0.7rem 1rem;
    border: none;
    background: #fff;
    color: #111;
    border-radius: 6px;
    font-weight: 600;
    cursor: pointer;
    transition: 0.3s;

    &:hover {
      background: #e5e5e5;
    }
  }

  @media (max-width: 900px) {
    grid-template-columns: 1fr 1fr;
  }

  @media (max-width: 600px) {
    grid-template-columns: 1fr;
    text-align: center;

    ul li {
      cursor: default;
    }

    button,
    input {
      max-width: 320px;
      margin-left: auto;
      margin-right: auto;
      display: block;
    }
  }
}


</style>