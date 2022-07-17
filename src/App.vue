<template><Portfolio /> <Card /></template>

<script>
import Portfolio from "./components/Portfolio.vue";
import Card from "./components/Card.vue";

export default {
  name: "App",
  components: {
    Portfolio,
    Card,
  },
};
</script>

<style>
body {
  background: rgba(52, 49, 72, 0.541);
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #343148ff;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
</style>
