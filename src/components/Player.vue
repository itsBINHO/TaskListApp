<template>
  <div class="footerButtons">
    <v-col class="footerCollumn">
      <div class="AlbumTrack">
        <img src="#"/>
      </div>
      <div class="player-controls">
        <i class="fa-solid fa-backward" title="Previous" id="prev"></i>
        <i class="fa-solid fa-play play-button" title="Play" id="play"></i>
        <i class="fa-solid fa-forward" title="Next" id="next"></i>
      </div>
      <div class="volumeBar"></div>
    </v-col>
    <v-col class="music-progress">
      <div class="player-progress" id="player-progress">
        <div class="progress" id="progress"></div>
        <div class="music-duration">
          <span id="current-time">0:00</span>
          <span id="duration">0:00</span>
        </div>
      </div>
    </v-col>
  </div>
</template>

<script>
export default {
  name: "Player",
  data: () => ({
    songs: [
      {
        
      }
    ]
  }),
  methods: {
    playMusic() {
      
    },
    pauseMusic() {
      
    },
    nextMusic() {
      
    },
    previousMusic() {
      
    },
  },
};
</script>

<style>
.footerCollumn {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  width: 100%;
}
.footerButtons {
  background-color: #3d1f1f;
  position: fixed;
  bottom: 0;
  width: 75%;
}
.player-controls {
  text-align: center;
  width: 200px;
}

.fa-solid {
  font-size: 25px;
  color: #fffbfb;
  margin-right: 30px;
  cursor: pointer;
  user-select: none;
  transition: all 0.3s ease;
}

.fa-solid:hover {
  filter: brightness(40%);
}

.play-button {
  font-size: 35px;
  position: relative;
  top: 3px;
}
.volumeBar {
  background-color: #8b8181;
  width: 100px;
}
.music-progress {
  display: flex;
  margin-left: 22%;
}
.player-progress{
    background-color: #fff;
    border-radius: 5px;
    cursor: pointer;
    margin: 0px 20px 3px;
    height: 4px;
    width: 45%;
}

.progress{
    background-color: #212121;
    border-radius: 5px;
    height: 100%;
    width: 0%;
    transition: width 0.1s linear;
}

.music-duration{
    position: relative;
    top: -25px;
    display: flex;
    justify-content: space-between;
}
</style>
