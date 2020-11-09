<template>
  <div class="container">
    <div class="jumbotron">
      <h1 class="display-3">Hello, world!</h1>
      <p class="lead">
        This is a simple hero unit, a simple jumbotron-style component for
        calling extra attention to featured content or information.
      </p>
      <hr class="my-4" />
      <!-- <p class="lead">
        <button type="button" class="btn btn-info">Agregar un Ingreso</button>
        <button type="button" class="btn btn-danger">Agregar un Egreso</button>
      </p> -->
      <div class="btn-group" role="group" aria-label="Basic example">
        <button type="button" class="btn btn-info" @click="modalIngreso">
          Agregar un Ingreso
        </button>
        <button type="button" class="btn btn-danger">Agregar un Egreso</button>
      </div>
    </div>
    <div class="container d-flex justify-content-between">
      <resumen />
      <ingresos />
      <egresos />
    </div>
  </div>
</template>
<script>
import Resumen from "../components/Resumen";
import Ingresos from "../components/Ingresos";
import Egresos from "../components/Egresos";
export default {
  components: {
    Resumen,
    Ingresos,
    Egresos,
  },
  methods: {
    modalIngreso() {
      window.$("#egresos").modal("show");
    },
  },
};
</script>
<style scoped></style>
