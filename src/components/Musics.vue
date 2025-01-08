<template>
  <div class="songList">
    <v-row class="card">
      <v-col v-for="(item, index) in items" :key="index" class="customList pa-4">
        {{ tier[index]?.number }}
        <div class="sizeBtn">
        <btn class="file">
          {{ item.name }}
        </btn>
      </div>
        <a href="https://open.spotify.com/intl-pt/artist/6qqNVTkY8uBg9cP3Jd7DAH" target="_blank">Billie Eilish</a>
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
        name: "WILDFLOWER",
        id: 1,
      },
      {
        name: "Lovely",
        id: 2,
      },
      {
        name: "CHIHIRO",
        id: 3,
      },
      {
        name: "Your Power",
        id: 4,
      },
      {
        name: "Ocean eyes",
        id: 5,
      },
    ],
    tier: [
      { number: "1",
        id: 1,
        },
      { number: "2",
        id: 2,
        },
      { number: "3",
        id: 3,
        },
      { number: "4",
        id: 4,
        },
      { number: "5",
        id: 5,
        },
      ],
    }),
  created() {
    this.syncTier();
  },
  methods: {
    syncTier() {
      // Garante que tier seguirá a ordem numérica de `items`
      this.tier = this.items
        .sort((a, b) => Number(a.id) - Number(b.id)) // Ordena os itens por ID numérico
        .map((item) => ({ number: String(item.id) })); // Cria um array tier
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
  width: 65vw;
}
.customList {
  display: flex;
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
  font-size: .8em;
  text-decoration: underline;
}
.customList:hover {
  background-color: #5e5e5e2f;
  cursor: pointer;
}
</style>