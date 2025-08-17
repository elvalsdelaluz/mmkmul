<script setup>
const props =defineProps({
     value: [String, Number],
     size: {
          type: Number,
          default:1
     }
});

</script>

<template>
     <div class="border text-center custom-cell" :class="`g-col-${size}`">
          {{ value }}
     </div>
</template>


<style>
.custom-cell{
     display: flex;
     justify-content: center;
     align-items: center;
     width: 3rem; /*Altura de la celda*/
     min-height: 3rem; /*Ancho de la celda*/
  }

</style>