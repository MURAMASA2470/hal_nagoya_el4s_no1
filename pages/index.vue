<template>
  
<v-layout column>

<v-container grid-list-xl>
  <eventList />
</v-container>

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
  components: {
    EventList
  }
}
</script>
