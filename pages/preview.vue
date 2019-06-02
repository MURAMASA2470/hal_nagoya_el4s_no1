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
        <v-img width="64" src="https://rr.img.naver.jp/mig?src=http%3A%2F%2Fimgcc.naver.jp%2Fkaze%2Fmission%2FUSER%2F20140512%2F11%2F1250381%2F1%2F588x388xb4e189c2fe54166f076d6256.jpg%2F300%2F600&twidth=300&theight=600&qlt=80&res_format=jpg&op=r" />
      </div>
    </div>

  </div>


  <v-carousel hide-delimiters hide-controls height="90vh" :interval="second" v-on:click="tap" :touch="tap">
    <v-carousel-item src="https://uds.gnst.jp/rest/img/k9e7wv5v0000/s_0034.jpg?t=1531897297"/>
    <v-carousel-item src="https://s3-ap-northeast-1.amazonaws.com/mag.nearly.do/item_getties/images/000/135/351/medium/8b1a2f53-5937-42ca-88bc-e63098c137f5.jpg?1529681226"/>
    <v-carousel-item src="https://housefoods-group.com/activity/e-mag/magazine/images/04/a.jpg"/>
  </v-carousel>

<!-- <v-container grid-list-xl>
  <eventList />

  <eventList />
</v-container> -->

</v-layout>
</template>

<script>
import EventList from '~/components/eventList.vue'

export default {
  data() {
    return {
      second: 6 * 1000, 

    }
  }, 
  methods: {
      tap: () => {
          alert(1);
      }, 
      profileTapped: () => {
          location.href="/";
      }
  }, 
  components: {
    EventList
  }
}
</script>
