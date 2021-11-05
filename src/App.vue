<template>
  <div id="app">
    <index></index>
  </div>
</template>

<script>
import Index from "./components/Index.vue";

export default {
  name: "App",
  components: {
    index: Index,
  },
};
</script>

<style>
#app {
  /* Container */
  padding-right: 15px;
  padding-left: 15px;
  margin-right: auto;
  margin-left: auto;
  display: flex;
  align-items: center;
  flex-direction: column;
  align-self: center;
  border-radius: 10px;
  /* Background */
  background: #4ca1af; /* fallback for old browsers */
  background: -webkit-linear-gradient(
    to right,
    #c4e0e5,
    #4ca1af
  ); /* Chrome 10-25, Safari 5.1-6 */
  background: linear-gradient(
    to right,
    #c4e0e5,
    #4ca1af
  ); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
}
</style>
