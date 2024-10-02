<script setup>

import Tetris from './components/Tetris.vue'
import { onMounted} from 'vue';

onMounted(() => {
    document.title = 'Tetris With Vue| Leka201' 

      const canvas = document.getElementById("tetris");
      const context = canvas.getContext("2d");
      context.scale(20, 20);

   });

</script>

<template>
   
   <Tetris/>    
   <div id= "score"></div>
   <canvas id = "tetris" width ="240" height="400"></canvas>

</template>

<style>

body{
   background: #202028; 
   color: #fff;
   font-family: sans-serif;
   font-size: 2em;
   text-align: center;
}

canvas{
   border: solid 0.2em #fff; 
   height: 90vh;
}

</style>


