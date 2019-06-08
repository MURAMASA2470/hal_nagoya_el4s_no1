<template>
  
<v-layout column>

  <!-- <videoPlayer path="http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4" /> -->

  <div>
    <v-img style="height:85vh;opacity:0.4;" src="https://uds.gnst.jp/rest/img/k9e7wv5v0000/s_0034.jpg?t=1531897297"/>
  </div>

  <div class="play-icon">
    <n-link to="/preview"><v-img src="https://cdn.discordapp.com/attachments/582438479317827584/586735402912841728/play-5063_92095300-a1b5-42aa-af42-8e2ff343fd58.svg"></v-img></n-link>
  </div>

</v-layout>
</template>

<style scoped>
  .play-icon {
    width: 100px;
    height: 100px;
    opacity: 0.8;
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    margin: auto;
  }
</style>


<script>

export default {
  data() {
    return {

    }
  }, 
  components: {
  }
}
</script>
