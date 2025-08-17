<script setup>
import MatrixCell from './MatrixCell.vue'
import { ref } from 'vue';

const props = defineProps({
  myprop: String
})

//Datos para las celdas
const cells = ref(Array.from({length: 16}, (_,i) =>({
  id: i,
  value: i+1,
  size: 1
})))
</script>

<template>
  <div>
    {{ props.myprop }}
    <div class="grid border p-2 custom-matrix">
        <MatrixCell
          v-for="(cell, index) in cells"
          :key="index"
          :value="cell.value"
          :size="cell.size"
        />
    </div>
  </div>
</template>

<style>
.custom-matrix{
  --bs-columns: 4; 
  --bs-gap: 0.1rem;
  width: 13.5rem; /*Tamaño del div que va a contener la matriz.*/
}
</style>