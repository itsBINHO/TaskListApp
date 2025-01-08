<template>
  <div class="songList d-flex">
    <v-row class="card">
      <v-col v-for="(item, index) in items" :key="index" class="customList">
        {{ tier[index]?.number }}
        <div class="sizeBtn">
          <btn class="file">
            {{ item.name }}
          </btn>
        </div>
        <a
          href="https://open.spotify.com/intl-pt/artist/6qqNVTkY8uBg9cP3Jd7DAH"
          target="_blank"
          >Billie Eilish</a
        >
        <div class="LogoList">
          <img :src="getLogoById(item.id)" alt="Logo" />
        </div>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: "Musics",
  data: () => ({
    items: [
      {
        name: "Bad Guy",
        id: 1,
      },
      {
        name: "Lovely",
        id: 2,
      },
      {
        name: "Ocean Eyes",
        id: 3,
      },
      {
        name: "Hot Lines",
        id: 4,
      },
    ],
    tier: [
      { number: "1", id: 1 },
      { number: "2", id: 2 },
      { number: "3", id: 3 },
      { number: "4", id: 4 },
    ],
    albumMusic: [
      {
        logoMusic: "src/assets/badGuyLogo.png",
        id: 1,
      },
      {
        logoMusic: "src/assets/lovelyLogo.png",
        id: 2,
      },
      {
        logoMusic: "src/assets/oceanEyesLogo.png",
        id: 3,
      },
      {
        logoMusic: "src/assets/hotLinesLogo.png",
        id: 4,
      },
    ],
  }),

  methods: {
    getLogoById(id) {
      const logoItem = this.albumMusic.find((album) => album.id === id);
      return logoItem ? logoItem.logoMusic : "";
    },
  },
};
</script>

<style>
.songList {
  padding: 1em;
  margin-left: 2em;
}
.card {
  display: flex;
  flex-direction: column;
}
.customList {
  display: flex;
  height: 4em;
  align-items: center;
}
.sizeBtn {
  width: 20%;
}
.file {
  padding: 1.7em;
}
.customList a {
  margin-left: 30%;
  color: #494444;
  font-size: 0.8em;
  text-decoration: underline;
}
.customList:hover {
  background-color: #5e5e5e2f;
  cursor: pointer;
}
.LogoList {
  display: flex;
  padding: 10px;
  margin-left: 39%;
}
.LogoList img {
  width: 60px;
  height: auto;
  object-fit: contain;
}
</style>
