<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <nav class="navbar navbar-light bg-light">
    <div class="container-fluid">
      <a class="navbar-brand"><img src="./assets/images/logo.png" alt="Logo de compañia mmkmul"></a>
      <button class="config-button" @click="openConfig">
        <img src="./assets/images/configurar.png" alt="Configuración">
      </button>
    </div>
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