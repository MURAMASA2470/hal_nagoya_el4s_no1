<template>
    <v-bottom-nav
      :value="true"
      absolute
    >
      <v-btn to="/home" color="yellow" flat >
        <span class=""></span>
        <v-icon>insert_emoticon</v-icon>
      </v-btn>

      <v-btn></v-btn>

      <a href="/addition" class="center-btn">
        <span class=""></span>
        <v-icon>add</v-icon>
      </a>

      <v-btn to="/mypage" color="yellow" flat >
        <span class=""></span>
        <v-icon>home</v-icon>
      </v-btn>

    </v-bottom-nav>
</template>

<style lang="css" scoped>
.center-btn {
  background-color: rgb(255, 208, 0);
  width: 100px;
  height: 100px;
  border-radius: 100%;
  position: absolute;
  top:-17px;
}

i {
  font-size: 2rem;
}

.center-btn > i {
  width: 100%;
  text-align: center;
  font-size: 4rem;
  color: white;
  line-height: 6rem;
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