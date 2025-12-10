<script setup>
    import { ref } from "vue"
defineProps(["imagem"]);

const liked = ref(false);
</script>

<template>
<div class="card">
<span @click="liked = !liked">{{ liked ? '❤️' : '🤍' }}</span>
    <img :src="imagem" alt="Imagem">
</div>
</template>

<style scoped lang ="scss">
.card{
    //border: solid;
    width: 35vw;
    img{
        width: 100%;
        height: 100%;
        border-radius: 10px
    };
    span{
        font-size: 2rem;
        cursor: pointer;
        position: relative;
        top: 50px;
    }
    
}

</style>