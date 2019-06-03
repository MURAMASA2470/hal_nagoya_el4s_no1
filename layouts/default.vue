<template>
  <v-app  style="height:100vh;">

    <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      app
    >
      <v-list>
        <v-list-tile
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-tile-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title v-text="item.title" />
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>

    <v-toolbar
      :clipped-left="clipped"
      fixed
      :manual-scroll="false"
      app
      color="#2FCB71"
    >
      <!-- <v-toolbar-side-icon @click="drawer = !drawer" /> -->
     
      <v-toolbar-title v-text="title" />

      <v-spacer />
      
    </v-toolbar>

    <v-content>
      <!-- <v-container> -->
        <nuxt />
      <!-- </v-container> -->
    </v-content>

    <v-footer :fixed="fixed" app>
      <BottomNav />
    </v-footer>

  </v-app>
</template>

<style scoped>
</style>


<script>
import BottomNav from '~/components/bottomNav.vue'

export default {
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      miniVariant: false,
      title: 'Fuji Design'
    }
  },
  components: {
    BottomNav
  }
}
</script>
