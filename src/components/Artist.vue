<template>
  <div id="perfil" class="d-flex ml-10 mt-10">
    <img :src="logo" :alt="nome">
  </div>
</template>

<script>

  export default {
    name: 'Artist',
    props: {
      nome: {
        type: String,
        required: true,
      },
    },
      data() {
        return {
          logo: 'src/assets/artist-img.png',
        }
      }
    }
</script>

<style>
  img.perfil {
    cursor: pointer;
  }
</style>