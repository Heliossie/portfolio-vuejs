<template>
  <div>
    <nav></nav>
    <portfolio></portfolio>
    <about></about>
    <contact></contact>
  </div>
</template>

<script>
import About from "./about-me/About.vue";
import Portfolio from "./portfolio/Portfolio.vue";
import Contact from "./contact/Contact.vue";
export default {
  name: "Index",
  components: {
    about: About,
    portfolio: Portfolio,
    contact: Contact,
  },
};
</script>

<style>
</style>