<template>
  <div class="hello">
    <h2>Filho abaixo</h2>
    <input type="checkbox" :checked="accTerm" v-model="accTerm" @change="$emit('aceitou', accTerm)">Aceita os termos?
  </div>
</template>

<script>
export default {
  name: "ComponenteFilho",
  data() {
    return {
      accTerm: false
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
button {
  padding: 20px;
  border: 0;
  border-radius: 5px;
  background: brown;
  color: white;
}
</style>
