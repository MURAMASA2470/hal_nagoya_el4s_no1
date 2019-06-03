<template>
  
<v-layout column>

  <!-- <videoPlayer path="http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4" /> -->

<v-container grid-list-xl>
  <eventList />
</v-container>

</v-layout>
</template>

<script>
import EventList from '~/components/eventList.vue'
import VideoPlayer from '~/components/video.vue'

export default {
  data() {
    return {

    }
  }, 
  components: {
    EventList, 
    VideoPlayer
  }
}
</script>
