<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Controls from './components/Controls.vue'
import MatrixBlocks from './components/MatrixBlocks.vue';

</script>

<template>
  <nav class="navbar navbar-base">
    <div class="container-fluid">
      <a class="text-logo">mmkmul</a>
      <button class="config-button" @click="openConfig">
        <img src="./assets/images/configurar.svg" alt="Configuración">
      </button>
    </div>
  </nav>
  <MatrixBlocks />
  <Controls />

</template>

<style>
.navbar-base {
  background: var(--color-background);  
  padding-top: 0.9rem;
  padding-left: 0.1rem; /* Creo que hay un padding por defecto */
  padding-right: 0.1rem; /* El padding left y right se ve si es mayor a 3 */
}

.text-logo {
  font-size: 1.8rem;  
  font-family: "Comfortaa", sans-serif;
  font-weight: 700;
}
</style>