<template>
  <div>
    <nav-bar/>
    <billetera-front />
  </div>
</template>

<script>
import BilleteraFront from "./views/BilleteraFront.vue";
import NavBar from './components/NavBar'

export default {
  name: "App",
  components: {
    BilleteraFront,
    NavBar
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
