<script setup>
import { RouterLink, RouterView } from 'vue-router'
// import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div>
    <div class="flex items-start min-h-screen bg-gray-100">
      <div class="hidden sm:flex sm:flex-col sticky top-0 z-10 bg-slate-900 min-h-screen border-r duration-300 w-16 lg:w-64">
        <div class="w-full bg-green-900 p-2">
          <h1 class="text-xl text-green-100 text-center font-semibold uppercase">Marven Alampayan</h1>
          <p class="text-lg text-gray-100 text-center font-normal">Semifinal Project</p>
        </div>
        <nav class="mt-4">
          <ul class="space-y-4">
            <li>
              <RouterLink to="/" class="flex items-center justify-center py-4 bg-slate-600 text-gray-300">Home</RouterLink>
            </li>
            <li>
              <RouterLink to="/about" class="flex items-center justify-center py-4 bg-slate-600 text-gray-300">Products</RouterLink>
            </li>
            <li>
              <RouterLink to="/about" class="flex items-center justify-center py-4 bg-slate-600 text-gray-300">Categories</RouterLink>
            </li>
            <li>
              <RouterLink to="/about" class="flex items-center justify-center py-4 bg-slate-600 text-gray-300">Transactions</RouterLink>
            </li>
            
          </ul>
        </nav>

        <div class="flex-grow flex items-end">
          <footer class="flex items-center justify-center flex-col p-4 bg-slate-600">
            <p class="text-gray-300 text-sm text-center">
              This is a laboratory file intended for training students in the use of VueJS 3 created by Benjie B. Lenteria for the students of Mater Dei College.
            </p>
            <p class="text-gray-300 text-sm text-center">Copyright © 2023.</p>
            <p class="text-gray-300 text-sm text-center">All rights reversed.</p>
          </footer>
        </div>
      </div>
      <div class="flex-1 min-h-screen overflow-hidden bg-green-200">
        <RouterView />
      </div>
    </div>
  </div>
</template>