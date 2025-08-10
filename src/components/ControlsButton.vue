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
.config-button img[alt="adelantar"] {
  width: 2.6rem;
  height: 2.6rem;
}
.config-button img[alt="rebobinar"] {
  width: 2.6rem;
  height: 2.6rem;
}
</style>
