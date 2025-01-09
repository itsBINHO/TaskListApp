<template>
  <main class="d-flex">
    <section>
      <div class="d-flex" id="containerTop">
        <Artist/>
      </div>
      <Library/>
    </section>
    <Aside/>
  </main>
</template>

<script>
</script>
<style>
  section {
    background: linear-gradient(to right,#000000, #3b1e1e, #6A2525);
    height: 100vh;
    width: 75vw;
    color: white;
  }
  html, body {
  margin: 0;
  padding: 0;
  overflow: hidden; /* Desativa a rolagem */
  height: 100%;
}
</style>