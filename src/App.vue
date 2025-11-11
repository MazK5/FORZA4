<script setup lang="ts">
import { ref } from 'vue'
/*
  ////////////////////////////////////////
    FORZA4 TABLE TODO
  /////////////////////////////////////////

 -move from app.vue to views
 -add code logic to make the game interactive
    -add logic for winning
    -add logic for turns
    -add player vs player / bot
    -animations when inserting elements ( it needs to fall down )
    -color for different players and background (when empty = ,p1= red, p2= yellow )
    -add restart button
    -add score board

  - save scores with pinia or cookies
  -use router to create different views ( home, game, settings, about us )
*/

const elementInserted = ref(0) ;

function insert() {
  console.log("insert called");
  elementInserted.value += 1 ;
}


</script>

<template>

  <h1>FORZA4 </h1>
  <h2> By maksym </h2>
  
  <p class ="generalText">
    Visit <a href="https://github.com/MazK5/FORZA4" target="_blank" rel="noopener">git project</a> to see the code repository.
  </p>

  <div id="forza4table">

    <div class="tbleRow">
      <!-- to change with a for i ? -->
      <P @click="insert"></P>
      <P @click="insert"></P>
      <P @click="insert"></P>
      <P @click="insert"></P>
      <P @click="insert"></P>
      <P @click="insert"></P>
      <P @click="insert"></P>
      <P @click="insert"></P>
      <P @click="insert"></P>
      <P @click="insert"></P>
    </div>

    <div class="tbleRow">
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
    </div>

    <div class="tbleRow">
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
    </div>

    <div class="tbleRow">
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
    </div>

    <div class="tbleRow">
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
    </div>

    <div class="tbleRow">
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
      <P>  </P>
    </div>

  </div>
  <p id="count"> Elements inserted: {{ elementInserted }} </p>

  <footer>
    <p id="author">Author: Maksym <br>
    <a href="mailto:"></a>Maksym@</p>
  </footer>

</template>
<style scoped>
</style>
