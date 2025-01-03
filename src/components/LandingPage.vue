<template>
  <main class="d-flex">
    <section class="d-flex">
      <div id="perfil" class="d-flex ml-10 mt-10">
        <img src="/src/assets/artist-img.png" alt="Billie Eilish" class="perfil">
      </div>
      <Info/>
      <Category/>
  </section>
  <aside class="d-flex">
    <div></div>
  </aside>
  </main>
</template>

<script>
  import Info from './Info.vue';
  import Category from './Category.vue';
</script>

<style>

  main {
    background: linear-gradient(to right,#000000, #2D1C1C, #6A2525);
    color: white;
  }

  img.perfil {
    cursor: pointer;
  }
</style>
