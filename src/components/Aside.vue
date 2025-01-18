<template>
  <div class="bar">
    <div class="titleBar">
      <h3>Groove</h3>
      <img src="/src/assets/menubar.svg" alt="Menu" />
      <h4>Search</h4>
    </div>
    <div class="menus">
      <v-col
        v-for="(item, index) in menuIcons"
        :key="index"
        class="colAside"
        :class="{
          'second-last': index === menuIcons.length - 2,
          last: index === menuIcons.length - 1,
        }"
      >
        <div class="iconsAside">
          <img :src="item.icon" alt="Menu Icon" />
        </div>
        <div class="listAside">
          <a href="#">{{ menuTitle[index]?.title }}</a>
        </div>
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
        icon: "src/assets/headphone.svg",
        id: 1,
      },
      {
        icon: "src/assets/explorer.svg",
        id: 2,
      },
      {
        icon: "src/assets/radio.svg",
        id: 3,
      },
      {
        icon: "src/assets/playBtn.svg",
        id: 4,
      },
      {
        icon: "src/assets/album.svg",
        id: 5,
      },
      {
        icon: "src/assets/profile.svg",
        id: 6,
      },
      {
        icon: "src/assets/song.svg",
        id: 7,
      },
      {
        icon: "src/assets/menubar.svg",
        id: 8,
      },
      {
        icon: "src/assets/menubar.svg",
        id: 9,
      },
    ],
    menuTitle: [
      {
        title: "Your Groove",
        id: 1,
      },
      {
        title: "Explore",
        id: 2,
      },
      {
        title: "Radio",
        id: 3,
      },
      {
        title: "Now Playing",
        id: 4,
      },
      {
        title: "Album",
        id: 5,
      },
      {
        title: "Artist",
        id: 6,
      },
      {
        title: "Songs",
        id: 7,
      },
      {
        title: "Playlist",
        id: 8,
      },
      {
        title: "Best of 2023",
        id: 9,
      },
    ],
  }),
};
</script>

<style>
.colAside {
  transition: font-size 0.2s linear, color 1s ease;
}
.colAside:hover {
  font-size: 1.1em;
  cursor: pointer;
}
.bar {
  background: linear-gradient(#993737, #8e5c5c);
  width: 25vw;
  position: relative;
  padding: 2.8em;
}
.titleBar {
  font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
    "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
}

.titleBar h3 {
  margin-bottom: 1em;
}
.titleBar h4 {
  margin-top: 1em;
}
.iconsAside {
  margin-left: -1em;
  height: 2.5em;
  margin-top: 1em;
}
.listAside {
  font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
    "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
  margin-left: 3em;
  margin-top: -2.2em;
}
.listAside a {
  color: black;
  font-size: 1.2em;
  text-decoration: none;
}
.second-last {
  margin-top: 2.5em;
  /* Adicione outros estilos para o penúltimo item */
}
@media (max-width: 1550px) {
  .bar {
    display: none;
  }
}
@media (max-width: 480px) {
  
}
</style>