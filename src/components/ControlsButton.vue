<script setup>
const props = defineProps({
  myprop: String
})

const path = new URL(`../assets/images/${props.myprop}.svg`, import.meta.url).href
</script>

<template>
  <button class="config-button" @click="$emit('prev')">
    <img :src="path" :alt="props.myprop" />
  </button>
</template>

<style>
.config-button {
  background: none;
  border: none;
  cursor: pointer;
  padding: 0;
  margin: 0;
}

.config-button img {
  width: 2rem;
  height: 2rem;
  display: block; /* Elimina espacio inferior de imágenes inline */
}
</style>
