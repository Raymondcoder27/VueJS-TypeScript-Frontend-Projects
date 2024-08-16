<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>

    <div class="items-center justify-center">
      <nav class="flex pr-3">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
  @import "@/assets/styles/app.css";
</style>
