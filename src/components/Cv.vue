<script setup>
  import { ref } from 'vue'

  defineProps({
    msg: String,

  })
</script>

<template>

<header class="flex fixed top-0 z-50 w-full border-b shadow-sm bg-gray-200">
  <div class="px-4 flex items-center justify-between max-w-7xl mx-auto">
    <!-- Logo -->
    <a href="/" class="text-lg font-semibold tracking-tight hover:opacity-80 transition">
      {{ msg }}
    </a>

    <!-- Menú escritorio -->
    <nav class="hidden md:flex space-x-6 text-sm font-medium">
      <a href="#inicio" class="hover:text-blue-600 transition">Inicio</a>
      <a href="#sobre" class="hover:text-blue-600 transition">Sobre mí</a>
      <a href="#proyectos" class="hover:text-blue-600 transition">Proyectos</a>
      <a href="#cv" class="hover:text-blue-600 transition">CV</a>
      <a href="#contacto" class="hover:text-blue-600 transition">Contacto</a>
    </nav>

    <!-- Menú móvil -->
    <details class="relative md:hidden">
      <summary
        class="list-none flex items-center gap-2 rounded-xl border px-3 py-2 text-sm cursor-pointer select-none"
      >
        <span>Menú</span>
        <!-- Ícono hamburguesa -->
        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24"
          stroke="currentColor" stroke-width="2">
          <path stroke-linecap="round" stroke-linejoin="round" d="M4 6h16M4 12h16M4 18h16" />
        </svg>
      </summary>
      <nav
        class="absolute right-0 mt-2 w-48 rounded-xl border bg-white shadow-lg flex flex-col py-2 text-sm font-medium"
      >
        <a href="#inicio" class="px-4 py-2 hover:bg-gray-50">Inicio</a>
        <a href="#sobre" class="px-4 py-2 hover:bg-gray-50">Sobre mí</a>
        <a href="#proyectos" class="px-4 py-2 hover:bg-gray-50">Proyectos</a>
        <a href="#cv" class="px-4 py-2 hover:bg-gray-50">CV</a>
        <a href="#contacto" class="px-4 py-2 hover:bg-gray-50">Contacto</a>
      </nav>
    </details>
  </div>
</header>


</template>

<style scoped>

</style>
