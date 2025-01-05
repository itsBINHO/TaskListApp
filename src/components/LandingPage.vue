<template>
  <main class="d-flex">
    <section>
      <div class="d-flex" id="containerTop">
        <Artist/>
        <Info/>
        <Category/>
      </div>
      <Library/>
      <Musics />
    </section>
    <Aside/>
  </main>
</template>

<style>
  section {
    background: linear-gradient(to right,#000000, #3b1e1e, #6A2525);
    height: 100vh;
    width: 75vw;
    color: white;
  }
</style>
