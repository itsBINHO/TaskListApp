<template>
    <main class="d-flex">
      <div id="perfil" class="d-flex ml-10 mt-10">
        <img src="/src/assets/artist-img.png" alt="Billie Eilish" class="perfil">
      </div>
      <div class="info">
        <h1 class="text-h3 font-weight-bold mt-11 ml-6 mb-10">Billie Eilish</h1>
        <p class="ml-7">With "Bad Guy", she became the first <br> 
          artist born in the 21st century and third <br>
          Gen Z artist <a href="#">MORE</a></p>
      </div>
      <div class="category">
        <h2>Dance/Pop</h2>
        <div class="buttons-track">
         <v-btn variant="plain"></v-btn>
         <v-btn variant="plain"></v-btn>
         <v-btn variant="plain"></v-btn>
         <v-btn variant="plain"></v-btn>
        </div>
      </div>
    </main>
</template>

<script setup>
  //
</script>

<style>

  main {
    background: linear-gradient(to right,#000000, #2D1C1C, #6A2525);
    color: white;
  }

  img.perfil {
    cursor: pointer;
  }
  a {
    text-decoration: none;
    color: #6687FF;
  }

  .category {
    margin-top: 80px;
    margin-left: 27vw;
  }
</style>
