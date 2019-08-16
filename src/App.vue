<template>
  <div id="app">
    <h2>Pai abaixo</h2>
    <h4>{{accepTerm}}</h4>
    <ComponenteFilho @aceitou="accepTerm = $event"/>
  </div>
</template>

<script>
import ComponenteFilho from "./components/ComponenteFilho";

export default {
  name: "App",
  components: {
    ComponenteFilho
  },
  data() {
    return {
      accepTerm: false
    };
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

h4 {
  color: red;
}
</style>
