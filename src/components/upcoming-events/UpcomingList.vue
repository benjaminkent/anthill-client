<template lang="pug">
  .upcoming-events-container
    h3
      | upcoming events
    .upcoming-list
    UpcomingEvent
</template>



<script>
import UpcomingEvent from "./UpcomingEvent"

export default {
  name: "UpcomingList",
  components: {
    UpcomingEvent
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

