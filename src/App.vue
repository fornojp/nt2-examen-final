<template>
  <div id="app">
    <section class="jumbotron container mt-4">
      <InputEditable />
      <Respuesta />
    </section>
  </div>
</template>

<script>
import InputEditable from "/src/components/InputEditable.vue";
import Respuesta from "/src/components/Respuestas.vue";
export default {
  name: "App",
  components: {
    InputEditable,
    Respuesta,
  },
};
</script>

<style></style>
