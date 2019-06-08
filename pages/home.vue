<template>
  
<v-layout column>

  <!-- <videoPlayer path="http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4" /> -->

  <div>
    <v-img style="height:85vh;opacity:0.4;" src="https://uds.gnst.jp/rest/img/k9e7wv5v0000/s_0034.jpg?t=1531897297"/>
  </div>

  <div class="play-icon">
    <n-link to="/preview"><v-img src="https://icon-pit.com/wp-content/uploads/2018/10/play_icon_764-300x300.png"></v-img></n-link>
  </div>

</v-layout>
</template>

<style scoped>
  .play-icon {
    width: 250px;
    height: 250px;
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
