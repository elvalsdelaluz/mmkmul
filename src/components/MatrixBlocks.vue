<script setup>
import MatrixRow from './MatrixRow.vue'
</script>

<template>
  <div class="grid" style="--bs-columns: 3; --bs-gap: 2rem;">
     <ControlsButton
        v-for="name in name_images"
        :myprop="name"
        :key="name.id"
      />
  </div>

</template>


<style>
</style>