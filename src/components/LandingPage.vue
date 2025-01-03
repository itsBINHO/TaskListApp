<template>
  <main class="d-flex">
    <section>
      <div class="d-flex" id="containerTop">
        <div id="perfil" class="d-flex ml-10 mt-10">
          <img src="/src/assets/artist-img.png" alt="Billie Eilish" class="perfil">
        </div>
        <Info/>
        <Category/>
      </div>
      <Library/>
    </section>
    <Aside/>
  </main>
</template>

<script></script>

<style>

  section {
    background: linear-gradient(to right,#000000, #3b1e1e, #6A2525);
    height: 100vh;
    width: 75vw;
    color: white;
  }

  img.perfil {
    cursor: pointer;
  }
</style>
