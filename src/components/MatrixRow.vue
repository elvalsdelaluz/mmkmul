<script setup>
import MatrixCell from './MatrixCell.vue'

const props = defineProps({
  myprop: String
})
</script>

<template>
  <p>"props.myprop"</p>
  <div class="grid border p-2" style="--bs-columns: 4; --bs-gap: 0.5rem;">
      <MatrixCell
        v-for="name in 16"
        :key="name.id"
      />
  </div>
</template>


<style>
</style>