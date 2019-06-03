<template>
    <div>
        <div class="profile">
            <v-img style="width:100vw;" src="http://ceskylove.com/wp-content/uploads/2016/12/mig2.jpg" />
            <v-img width="64" class="flag" src="https://rr.img.naver.jp/mig?src=http%3A%2F%2Fimgcc.naver.jp%2Fkaze%2Fmission%2FUSER%2F20140512%2F11%2F1250381%2F1%2F588x388xb4e189c2fe54166f076d6256.jpg%2F300%2F600&twidth=300&theight=600&qlt=80&res_format=jpg&op=r" />

            <v-avatar size="128px">
                <img src="https://cdn.discordapp.com/avatars/491812248134877188/906ab4aac87dd2d88ddb0a6a2df508dc.png?size=128" alt="avater">
            </v-avatar>
            <div class="string">
                <h2>ししょう</h2>
                <span>韓国に住んでいる凄腕催眠術師です</span>
            </div>
        </div>

        <v-container grid-list-sm fluid>
          <v-layout row wrap>
            <v-flex
              v-for="n in 9"
              :key="n"
              xs4
              d-flex
            >
              <v-card flat tile class="d-flex">
                <v-img
                  :src="`https://picsum.photos/500/300?image=${n * 5 + 10}`"
                  :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 10}`"
                  aspect-ratio="1"
                  class="grey lighten-2"
                >
                  <template v-slot:placeholder>
                    <v-layout
                      fill-height
                      align-center
                      justify-center
                      ma-0
                    >
                      <v-progress-circular indeterminate color="grey lighten-5"></v-progress-circular>
                    </v-layout>
                  </template>
                </v-img>
              </v-card>
            </v-flex>
          </v-layout>
        </v-container>

    </div>
</template>

<style scoped>

.profile {
    position: relative;
    width: 100vw;
}

    .flag {
        position: absolute;
        right: 20px;
        top: 20px;
    }

    .v-avatar {
        position: absolute;
        left: 0;
        right: 0;
        bottom: 60px;
        margin: auto;
    }

    .string {
        text-align: center;
        margin: 35px 0 0 0;
    }
.gallery {
    
}
</style>

<script>
export default {
    data: () => {
        return {

        }
    }
}
</script>
