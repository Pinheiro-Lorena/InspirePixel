<script setup>
import { Icon } from '@iconify/vue';
import logo from '../assets/logo.png'
</script>

<template>
<header>
    <img :src="logo" alt="Logo">

    <nav>
        <ul>
        <li>
            <a href="">
                <Icon class="icon-search"   icon="material-symbols:search"/>
            </a>
        </li><a href="">Inicio</a>
        <li>
           
        </li><a href="">Galeria</a>
        <li>
            
        </li><a href="">Favoritos</a>
        
        <li>
            <a href="">
                <Icon class="icon"   icon="material-symbols:person"/>
            </a>
        </li>
        </ul>
    </nav>
</header>
</template>

<style scoped lang ="scss">
header{
    //border: solid;
    display: flex;
   justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    margin: 2rem;

    ul{
        display: flex;
        gap: 1rem;
        justify-content: space-between;
        flex-wrap: wrap;
        list-style: none;
        
    }
    a{
        text-decoration: none;
        color: black;
        font-size: 1.2rem;
        align-items: center;
    }
}

@media (max-width: 992px) {
  header {
    div {
      width: 55%;
    }

    ul {
      justify-content: center;
    }

    a {
      font-size: 1rem;
    }
  }
}


</style>