<script setup>
import MatrixRow from './MatrixRow.vue'

const name_matrix = ["A","B", "C"]
</script>

<template>
  <div class="grid border custon-matrix-block">
     <MatrixRow
        v-for="name in name_matrix"
        :myprop="name"
        :key="name.id"
      />
  </div>

</template>


<style>

.custon-matrix-block{
  --bs-columns: 3;
  --bs-gap: 6rem;
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 75vh;   /*No se si esto esta bien, es para que los botones esten más abajo*/
}
</style>