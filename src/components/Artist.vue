<template>
  <div id="perfil" class="d-flex ml-10 mt-10">
    <img :src="logo" alt="Billie Eilish">
  </div>
  <Info/>
  <Category/>
</template>

<script>
import Info from './Info.vue';
import Category from './Category.vue';

  export default {
    name: 'Artist',
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