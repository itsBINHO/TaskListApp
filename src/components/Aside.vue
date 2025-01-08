<template>
  <div class="bar">
    <div class="titleBar">
      <h3>Groove</h3>
      <img src="/src/assets/menubar.svg" alt="Menu" />
      <h4>Search</h4>
    </div>
    <div class="menus">
      <v-col>
        <div class="iconsAside"></div>
        <div class="listAside"></div>
        <div class="playlistsAside"></div>
      </v-col>
    </div>
  </div>
</template>

<script>
export default {
  name: "Aside",
  data: () => ({
    menuIcons: [
      {
        icon: '',
        id: 1,
      },
      {
        icon: '',
        id: 2,
      },
      {
        icon: '',
        id: 3,
      },
      {
        icon: '',
        id: 4,
      },
      {
        icon: '',
        id: 5,
      },
      {
        icon: '',
        id: 6,
      },
      {
        icon: '',
        id: 7,
      },
    ],
    menuTitle: [
      {
        title: 'Your Groove',
        id: 1,
      },
      {
        title: 'Explore',
        id: 2,
      },
      {
        title: 'Radio',
        id: 3,
      },
      {
        title: 'Now Playing',
        id: 4,
      },
      {
        title: 'Album',
        id: 5,
      },
      {
        title: 'Artist',
        id: 6,
      },
      {
        title: 'Songs',
        id: 7,
      },
    ]
  })
}
</script>

<style>
.bar {
  background: linear-gradient(#993737, #8e5c5c);
  width: 25vw;
  position: relative;
  padding: 2.8em;
}
.titleBar {
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
}

.titleBar h3 {
  margin-bottom: 1em;
}
.titleBar h4 {
  margin-top: 1em;
}
.menus {
  background-color: aqua;
}
</style>
