<template lang="pug">
  .upcoming-events-container
    h3
      | upcoming events
    .upcoming-list
    UpcomingEvent(
      v-for="events in events"
      :events="events"
    )
</template>



<script>
import axios from 'axios'
import events from "./upcoming-list.json"
import UpcomingEvent from "./UpcomingEvent"

export default {
  name: "UpcomingList",
  components: {
    UpcomingEvent
  },
  data () {
    return {
      events
    }
  },
  mounted () {
    axios
      .get('localhost:3030/events.json')
      .then(response => (this.events = response))
  }
}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Josefin+Sans');

.upcoming-events-container {
  background-color: #000;
  padding-bottom: 10px;
}

h3 {
  padding: 10px 0 0 10px;
  margin: 0;
  color: #07efb5;
  font-family: 'Josefin Sans', sans-serif;
}
</style>

