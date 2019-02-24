<template lang="pug">
  .upcoming-events-container
    h3
      | upcoming events
    .upcoming-list
    UpcomingEvent(
      v-for="event in events"
      :event="event"
    )
</template>



<script>
import axios from 'axios'
import UpcomingEvent from "./UpcomingEvent"

export default {
  name: "UpcomingList",
  components: {
    UpcomingEvent
  },
  data () {
    return {
      events: null
    }
  },
  mounted () {
    axios
      .get('http://localhost:3030/api/events')
      .then(response => this.events = response.data)
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

