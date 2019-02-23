<template lang="pug">
  .event-item-container
    h1.event-title
      | {{ event.name }}
    .event-details
      img.event-image(src="@/assets/tacos.jpeg")
      ul
        li
          | Description: {{ event.description }}
        li
          | Venue: {{ event.venue }}
        li
          | City: {{ event.city }}
        li
          | Date: {{ event.date }}
</template>

<script>
export default {
  name: "UpcomingEvent",
  props: {
    event: Object
  }
}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Josefin+Sans');

.event-item-container {
  display: flex;
  flex-direction: column;
  margin: 15px 10px;
  background-color: #161616;
  border-radius: 4px;
  font-family: 'Josefin Sans', sans-serif;
}

.event-title {
  margin: 5px 0 0 5px;
  color: #f0c808;
}

.event-details {
  display: flex;
}

img.event-image {
  height: 200px;
  margin: 5px 0 5px 5px;
  border-radius: 4px;
}

ul {
  list-style-type: none;
  padding-left: 10px;
}

li {
  color: #F0C808;
  padding-bottom: 10px;
}
</style>
