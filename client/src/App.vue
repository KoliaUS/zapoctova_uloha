<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from '@/components/HelloWorld.vue'
import navigation from "@/components/navigation.vue";
</script>

<template>
  <header>
    <navigation></navigation>
  </header>

  <RouterView />
</template>

<style>

</style>
