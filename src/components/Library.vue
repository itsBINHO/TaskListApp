<template>
  <h2 class="title">In library</h2>
  <div id="containerLibrary">
    <img src="/src/assets/capaAlbum.png" alt="Logo Album">
    <div class="albumInfo">
      <h2>Super Cell</h2>
      <p>2019</p>
      <p>4 songs</p>
      <div class="buttons-track d-flex mt-2 ">
      <v-btn variant="plain">
        <a href="#">
          <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M29.3113 13.8838L11.3013 2.8675C10.9236 2.63725 10.4915 2.51133 10.0493 2.5026C9.60702 2.49387 9.17036 2.60264 8.78387 2.81781C8.39739 3.03297 8.07491 3.34683 7.84936 3.72735C7.6238 4.10787 7.50325 4.54142 7.5 4.98375V27.0163C7.50325 27.4586 7.6238 27.8921 7.84936 28.2727C8.07491 28.6532 8.39739 28.967 8.78387 29.1822C9.17036 29.3974 9.60702 29.5061 10.0493 29.4974C10.4915 29.4887 10.9236 29.3628 11.3013 29.1325L29.3113 18.1163C29.6744 17.8952 29.9746 17.5844 30.1828 17.2138C30.3911 16.8431 30.5005 16.4251 30.5005 16C30.5005 15.5749 30.3911 15.1569 30.1828 14.7862C29.9746 14.4156 29.6744 14.1048 29.3113 13.8838ZM10.5 26.1063V5.89375L27.02 16L10.5 26.1063Z" fill="#F8F8F8"/>
          </svg>
        </a>
      </v-btn>
      <v-btn variant="plain">
        <a href="#">
          <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M32 18.2857H18.2857V32H13.7143V18.2857H0V13.7143H13.7143V0H18.2857V13.7143H32V18.2857Z" fill="#F8F8F8"/>
          </svg>
        </a>
      </v-btn>
      </div>
    </div>
  </div>
  <Musics/>
</template>

<script>
import Musics from './Musics.vue';

  export default {
    name: 'Library'
  }
</script>

<style>
  #containerLibrary {
    display: flex;
    padding: 2em;
    margin-left: 3rem;
  }

  h2.title {
    margin-top: 3rem;
    margin-left: 6rem;
  }

  .albumInfo {
    display: flex;
    flex-direction: column;
    margin-left: 5rem;
  }

  .buttons-track {
    display: flex;
    margin-left: -1em;
    gap: 2em;
  }

  p {
    color: #987878;
    padding: 3px;
    margin-bottom: 2px;
  }
</style>