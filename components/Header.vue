<template>
    <header class="bg-gray-800 text-white p-4">
      <div class="container mx-auto flex justify-between items-center">
        <h1 class="text-3xl font-bold">Lucidium Studios</h1>
        <nav>
          <ul class="flex space-x-6">
            <li><a href="/" class="hover:text-yellow-400">Home</a></li>
            <li><a href="/about" class="hover:text-yellow-400">About</a></li>
            <li><a href="/portfolio" class="hover:text-yellow-400">Portfolio</a></li>
            <li><a href="/contact" class="hover:text-yellow-400">Contact</a></li>
          </ul>
        </nav>
      </div>
    </header>
  </template>
  
  <script>
  export default {
    name: 'Header'
  }
  </script>
  
  <style scoped>
  /* You can add specific header styling here */
  </style>
  