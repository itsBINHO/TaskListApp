<template>
  <main class="d-flex">
    <section>
      <div class="d-flex" id="containerTop">
        <Artist :nome="nome"/>
      </div>
      <Library/>
    </section>
    <Aside/>
  </main>
</template>

<script>
import Artist from './Artist.vue';
</script>
<style>
  section {
    background: linear-gradient(to right,#000000, #3b1e1e, #6A2525);
    height: 100vh;
    width: 75vw;
    color: white;
  }
</style>
