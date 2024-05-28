<template>
  <TopBar/>
  <RouterView/>
</template>

<script setup>
import { RouterView } from 'vue-router'
import TopBar from "@/components/TopBar.vue";
</script>

<style>
body {
  background-color: #101524;
}
</style>
