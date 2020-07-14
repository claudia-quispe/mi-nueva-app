<template>
  <div id="lista">
    <h3>Discos que {{ nombre }} podría tener:</h3>
        <ol>
            <li v-for="(lista1, i) in discos1" v-bind:key="i">{{ lista1 }}</li>
        </ol>
  </div>
</template>

<script>

export default {
  name: 'Lista',
  data:function () {
    return {
      nombre: 'Rebeca', 
      discos1: ['Coastal Grooves', 'Cupid Deluxe', 'Freetown Sound', 'Negro Swan', 'Angel`s Pulse']
    }
  }
}
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  padding: 30px;
  background-color:cadetblue;
}


</style>
