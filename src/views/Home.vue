<template lang="pug">
  .home
    Header
    Hero
    RecentEvents
</template>

<script>
import Header from "@/components/Header";
import Hero from "@/components/Hero";
import RecentEvents from "@/components/RecentEvents"

export default {
  name: "Home",
  components: {
    Header,
    Hero,
    RecentEvents
  }
};
</script>
