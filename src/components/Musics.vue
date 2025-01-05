<template>
  <!-- <div class="songList d-block" style="background-color: transparent">
    <v-card>
      <v-list
        class="customList"
        style="background-color: transparent"
        :items="items"
        item-title="name"
        item-value="id"
      ></v-list>
    </v-card>
  </div> -->

  <div class="songList d-block">
    <v-card>
      <v-list
        class="customList"
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
    ],
  }),
};
</script>

<style>
.songList .v-list-item {
  background-color: red;
}

.v-list-item:hover {
  background-color: #0000001c;
  cursor: pointer;
}

.songList .v-list-item-title {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  font-weight: bold;
  color: aliceblue;
}
</style>
