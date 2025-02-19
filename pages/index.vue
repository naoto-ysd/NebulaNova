<template>
  <div class="container">
    <h1>Welcome to My Nuxt + TypeScript App</h1>
    <p>This is a simple Nuxt 3 application using TypeScript.</p>
    <button @click="handleClick">Click Me</button>
  </div>
</template>

<script setup lang="ts">
const handleClick = (): void => {
  console.log('Button clicked!')
}
</script>

<style scoped>
.container {
  max-width: 800px;
  margin: 0 auto;
  padding: 2rem;
  text-align: center;
  font-family: Arial, sans-serif;
}
</style>
