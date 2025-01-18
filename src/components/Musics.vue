<template>
  <div class="songList d-flex">
    <v-row class="card">
      <v-col v-for="(music, index) in music" :key="index" class="customList">
        {{ music.tier }}
        <div class="sizeBtn">
          <btn class="file">
            {{ music.name }}
          </btn>
        </div>
        <a
          href="https://open.spotify.com/intl-pt/artist/6qqNVTkY8uBg9cP3Jd7DAH"
          target="_blank"
          >Billie Eilish</a
        >
        <div class="LogoList">
          <img :src="music.logoMusic" alt="Logo" />
        </div>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: "Musics",
  data: () => ({
    music: [
      {
        name: "Bad Guy",
        id: 1,
        tier: "1",
        logoMusic: "src/assets/badGuyLogo.png",
        path: "src/assets/BillieEilish-badguy.mp3",
      },
      {
        name: "Lovely",
        id: 2,
        tier: "2",
        logoMusic: "src/assets/lovelyLogo.png",
        path: "src/assets/BillieEilish-lovely.mp3",
      },
      {
        name: "Ocean Eyes",
        id: 3,
        tier: "3",
        logoMusic: "src/assets/oceanEyesLogo.png",
        path: "src/assets/BillieEilish-OceanEyes.mp3",
      },
      {
        name: "hotline",
        id: 4,
        tier: "4",
        logoMusic: "src/assets/hotLinesLogo.png",
        path: "src/assets/BillieEilish-hotline.mp",
      },
    ],
  }),
}
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
