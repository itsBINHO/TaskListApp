<template>
  <div class="songList d-block">
    <v-card class="ml-11 bg-transparent">
      <v-list
        class="customList bg-transparent"
        :items="items"
        item-title="name"
        item-value="id"
      ></v-list>
    </v-card>
  </div>
</template>

<script>
export default {
  name: "Musics",
  data: () => ({
    items: [
      {
        name: "1 WILDFLOWER",
        id: 1,
      },
      {
        name: "2 Lovely",
        id: 2,
      },
      {
        name: "3 CHIHIRO",
        id: 3,
      },
      {
        name: "4 Your Power",
        id: "4"
      },
      {
        name: "Ocean eyes",
        id: "5"
      },
      {
        name: "6 TV",
        id: "6"
      }
    ],
  }),
};
</script>

<style>
.songList .v-list-item {
  gap: 1em;
  margin-top: 0.5em;
}

.v-list-item:hover {
  background-color: #7513131c;
  cursor: pointer;
}

.songList .v-list-item-title {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  font-weight: bold;
  color: aliceblue;
  padding: 0.2em;
}
</style>
