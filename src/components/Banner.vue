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

<style scoped lang ="scss">
.banner{
    //border: solid;
    display: flex;
    justify-content: space-between;
    margin: 2rem;

    h1{
        font-size: 2.8rem;
    }
    span{
        color:#E1306C;
        //font-weight: bold;
        font-size: 4.5rem;
    }

    div{
        border: solid;
        width: 50%;
        align-items: center;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }
}

</style>