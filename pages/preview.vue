<template>
  
<v-layout column>

  <div style="position:absolute;padding:20px;width:100vw;z-index:999;">
    <!-- <v-progress-linear value="60" indeterminate></v-progress-linear> -->
    
    <div class="profile">
      <div style="float:left;" class="person" v-on:click="profileTapped">
        <v-avatar>
          <img src="https://cdn.discordapp.com/avatars/491812248134877188/906ab4aac87dd2d88ddb0a6a2df508dc.png?size=256" alt="avater">
        </v-avatar>
        <span>ししょう</span>
      </div>
      <v-spacer></v-spacer>
      <div style="float:right;" class="country">
        <v-icon color="red" style="margin-right:10px;" x-large @click="favState = !favState">favorite{{ !favState ? '_border' : '' }}</v-icon>
        <v-img width="64" style="float:right;" src="https://rr.img.naver.jp/mig?src=http%3A%2F%2Fimgcc.naver.jp%2Fkaze%2Fmission%2FUSER%2F20140512%2F11%2F1250381%2F1%2F588x388xb4e189c2fe54166f076d6256.jpg%2F300%2F600&twidth=300&theight=600&qlt=80&res_format=jpg&op=r" />
      </div>
    </div>

  </div>


  <carousel
    :per-page="1"
    :autoplay="true"
    :loop="true"
    :paginationEnabled="false"
    :autoplay-timeout="4000"
    >
    <slide style="height:88vh;"><v-img style="height:100%;" src="https://uds.gnst.jp/rest/img/k9e7wv5v0000/s_0034.jpg?t=1531897297"/></slide>
    <slide style="height:88vh;"><v-img style="height:100%;" src="https://s3-ap-northeast-1.amazonaws.com/mag.nearly.do/item_getties/images/000/135/351/medium/8b1a2f53-5937-42ca-88bc-e63098c137f5.jpg?1529681226"/></slide>
    <slide style="height:88vh;"><v-img style="height:100%;" src="https://housefoods-group.com/activity/e-mag/magazine/images/04/a.jpg"/></slide>
  </carousel>

<!-- <v-container grid-list-xl>
  <eventList />

  <eventList />
</v-container> -->

</v-layout>
</template>

<style scoped>
</style>


<script>
import EventList from '~/components/eventList.vue'
import Carousel from 'vue-carousel/src/Carousel.vue'
import Slide from 'vue-carousel/src/Slide.vue'

export default {
  data() {
    return {
      second: 6 * 1000, 
      favState: false
    }
  }, 
  methods: {
      tap: (e) => {
          console.log(e);
      }, 
      profileTapped: () => {
          location.href="/mypage";
      }
  }, 
  components: {
    EventList,
    Carousel,
    Slide
  }
}
</script>
