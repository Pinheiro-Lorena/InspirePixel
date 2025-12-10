<script setup>
import Card from './Card.vue';

import axios from "axios";

//importamos o ref do vue
import { ref } from "vue";

//criamos uma variavel reativa para armazenar as imagens
const imagens = ref([]);

//função para buscar as imagens da api
async function carregarImagens () {
   const res = await axios.get("https://picsum.photos/v2/list?page=3&limit=60")

   imagens.value = res.data;
   console.log(res)
}

carregarImagens();
</script>

<template>
<h2>Inspire-se:</h2>
<section class="inspire">
<Card
v-for="img in imagens"
:imagem="img.download_url"
/>


</section>
</template>

<style scoped lang ="scss">
.inspire {
    display: flex;
    border-radius: 20px;
    flex-wrap: wrap;
    gap: 3rem;
    justify-content: center;
    

}
</style>