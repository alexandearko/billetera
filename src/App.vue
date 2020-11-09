<template>
  <div>
    <nav-bar />
    <billetera-front />
    <modal-ingreso />
    <modal-egreso />
  </div>
</template>

<script>
import BilleteraFront from "./views/BilleteraFront.vue";
import NavBar from "./components/NavBar";
import ModalIngreso from "./modals/ModalIngreso";
import ModalEgreso from "./modals/ModalEgreso";

export default {
  name: "App",
  components: {
    BilleteraFront,
    NavBar,
    ModalIngreso,
    ModalEgreso,
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
