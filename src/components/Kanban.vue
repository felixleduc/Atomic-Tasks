<script setup lang="ts">
//import { ref } from 'vue'
//const count = ref(0)
//defineProps<{ msg: string }>()

const columns = [
  {
    name: "Aujourd'hui",
  },
  {
    name: "Demain",
  },
  {
    name: "Cette semaine",
  },
  {
    name: "Ce mois-ci",
  },
  {
    name: "En attente",
  },
]
</script>

<template>
  <div class="container h-screen">
    <h1 class="py-6">Kanban board</h1>
    <div class="flex gap-3 h-5/6">
      <div v-for="column in columns" class="text-center flex-1 bg-slate-300">
        <h2 class=" py-4">{{ column.name }}</h2>
        <img src="../assets/plus-icon.svg" alt="Add a card image" class="w-10 mx-auto">
      </div>
    </div>
  </div>
</template>

<style scoped>
</style>