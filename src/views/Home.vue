<template lang="pug">
  .home
    Header
    Hero
    UpcomingList
</template>

<script>
import Header from "@/components/Header";
import Hero from "@/components/Hero";
import UpcomingList from "@/components/upcoming-events/UpcomingList"

export default {
  name: "Home",
  components: {
    Header,
    Hero,
    UpcomingList
  }
};
</script>
