<template>
  <section class="src-components-input-editable">
    <span>Color: <input type="text" v-model="color" class="mr-3" /></span>
    <span>Fondo: <input type="text" v-model="fondo" class="mr-3" /></span>
    <span>Size: <input type="number" v-model="size" /></span>
    <hr />
    <span
      >Texto:
      <input type="text" :style="getEstilo(color, fondo, size)" v-model="texto"
    /></span>
    <br />
    <br />
    <p v-if="this.texto != ''">Cantidad de palabras: {{ cantPalabras }}</p>
  </section>
</template>

<script>
export default {
  name: "src-components-input-editable",
  props: [],
  mounted() {},
  data() {
    return {
      color: "",
      fondo: "",
      size: "",
      texto: "",
    };
  },
  methods: {
    getEstilo(colorLetra, colorFondo, size) {
      return {
        color: colorLetra,
        backgroundColor: colorFondo,
        fontSize: size + "px",
      };
    },
  },
  computed: {
    cantPalabras() {
      let cantidad = this.texto.split(" ");
      return this.texto == "" ? 0 : cantidad.length;
    },
  },
};
</script>

<style scoped lang="css"></style>
