<template>
  <div id="app">
    <!-- <VueRouter></VueRouter> -->
    <NavBar title="my title"/>
  </div>
</template>

<script>
import VueRouter from "vue-router";
import NavBar from "./components/NavBar";
export default {
  name: "App",
  components: {
    NavBar,
    VueRouter
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
