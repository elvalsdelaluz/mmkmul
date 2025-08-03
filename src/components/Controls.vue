<script setup>
import ControlsButton from './ControlsButton.vue'

const name_images = ["adelantar", "iniciar", "pausar", "rebobinar"]
</script>

<template>
    <div class="controls">
      <ControlsButton
        v-for="name in name_images"
        :myprop="name"
        :key="name.id"
      />
    </div>
</template>

<style>

.controls {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 0.5rem;
  margin-top: 1rem;
}

</style>