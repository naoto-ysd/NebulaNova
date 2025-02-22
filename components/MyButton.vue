<template>
    <button class="my-button" @click="$emit('click')">
      {{ label }}
    </button>
  </template>
  
  <script setup lang="ts">
  import { defineProps } from 'vue'
  
  const props = defineProps<{
    label: string
  }>()
  </script>
  
  <style scoped>
  .my-button {
    padding: 0.5rem 1.5rem;
    border: 2px solid #1d4ed8;
    border-radius: 4px;
    background-color: #fff;
    color: #1d4ed8;
    cursor: pointer;
    transition: background-color 0.3s;
  }
  .my-button:hover {
    background-color: #1d4ed8;
    color: #fff;
  }
  </style>
  