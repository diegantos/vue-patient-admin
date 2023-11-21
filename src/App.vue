<script setup>
  import Header from './components/Header.vue'
  import Formulario from './components/Formulario.vue'
  import { ref } from 'vue';

  const pacientes = ([])

</script>

<template>
  <div class="container mx-auto mt-20">
    <Header />
    
    <div class="mt-12 md:flex">
      <Formulario />

      <div class="md:w-1/2 md:h-screen overflow-y-scroll">
        <h3 class="font-black text-3xl text-center">Administra tus pacientes</h3>
        <div v-if="pacientes.length > 0"></div>
        <div v-else class="mt-20 text-2xl text-center">No hay pacientes</div>
      </div>
    </div>
  </div>
</template>
