<template>
  <section class="src-components-respuestas container mt-4">
    <hr />
    <h1>Preguntas</h1>
    <table class="table table-dark">
      <thead>
        <tr>
          <th scope="col">Numero de Pregunta</th>
          <th scope="col">Respuesta</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th scope="row">¿Que es Axios?</th>
          <td>B- Es una biblioteca de cliente http</td>
        </tr>
        <tr>
          <th scope="row">Con Axios se pueden implementar los verbos</th>
          <td>C- Get, Post, Put y Delete</td>
        </tr>
        <tr>
          <th scope="row">¿Que es Vuex?</th>
          <td>
            B- Es una librería que maneja el estado de nuestras aplicaciones
          </td>
        </tr>
        <tr>
          <th scope="row">
            Las acciones en su implementación permiten lógica ...
          </th>
          <td>D- Asincrónica y sincrónica</td>
        </tr>
        <tr>
          <th scope="row">Las mutaciones ...</th>
          <td>D- Alteran directamente el estado de nuestra aplicación</td>
        </tr>
      </tbody>
    </table>
  </section>
</template>

<script>
export default {
  name: "src-components-respuestas",
  props: [],
  mounted() {},
  data() {
    return {};
  },
  methods: {},
  computed: {},
};
</script>
