<template>
    <v-bottom-nav
      :active.sync="bottomNav"
      :value="true"
      absolute
    >
      <v-btn v-for="(item, i) in navItems" :key="i" :to="item.to" :color="item.color" flat >
        <span v-text="item.title" class=""></span>
        <v-icon v-text="item.icon"></v-icon>
      </v-btn>

    </v-bottom-nav>
</template>

<script>

  export default {
    data () {
      return {
        bottomNav: 'Home', 
        navItems: [
          {
            icon: 'home', 
            title: 'Home', 
            color: 'teal', 
            to: '/'
          }, 
          {
            icon: 'favorites', 
            title: 'Secondary', 
            color: 'teal', 
            to: '/secondary'
          }
        ]
      }
    }
  }
</script>