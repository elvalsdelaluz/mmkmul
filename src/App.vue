<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <nav class="app-header">
      <h1>mmkmul</h1>
      <button class="config-button" @click="openConfig">
        <img src="./assets/images/configurar.png" alt="Configuración">
      </button>
  </nav>
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
  width: 24px;
  height: 24px;
  display: block; /* Elimina espacio inferior de imágenes inline */
}
</style>