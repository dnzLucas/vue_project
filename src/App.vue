<script setup>
import { ref } from 'vue'
const contador = ref(0)
function reset(){
  contador.value=0
}


</script>

<template>
<div class="counter-content">
  <button @click="contador++">+</button>
  <button @click="contador--">-</button>
  <button @click="reset" >Reiniciar</button>
  <p>Valor do contador: {{ contador }}</p>
</div>
</template>

<style scoped>

button {
  margin: 11px;
  width: 200px;
  height: 50px;
  border-radius: 20px;
  font-size: 2em;
  border: 0;
  transition: all 0.2s;

}
button:hover {
  background-color: black;
  color: white;
}

.counter-content{
  display: block;
  text-align: center;
  justify-content: center;
}

</style>
