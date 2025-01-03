<template>
  <h2 class="title">In library</h2>
  <div id="containerLibrary">
    <img src="/src/assets/capaAlbum.png" alt="Logo Album">
    <div class="albumInfo">
      <h2>Super Cell</h2>
      <p>2019</p>
      <p>4 songs</p>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'Library'
  }
</script>

<style>
  #containerLibrary {
    display: flex;
    padding: 2em;
    margin-left: 2rem;
  }

  h2.title {
    margin-top: 4rem;
    margin-left: 4rem;
  }

  .albumInfo {
    display: flex;
    flex-direction: column;
    margin-left: 4rem;
  }

  p {
    color: #987878;
  }
</style>