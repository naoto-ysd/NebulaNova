<template>
  <div class="api_demo">
    <h1>API Demo</h1>
    <p v-if="data">{{ data.message }}</p>
    <p v-else>Loading...</p>
  </div>
</template>
  
<script setup lang="ts">
const { data, error } = await useFetch<{ message: string }>('/api/hello');

if (error.value) {
  console.error('Error fetching API:', error.value);
}
</script>

<style scoped>
.api_demo {
  text-align: center;
  padding: 2rem;
  }
</style>
  