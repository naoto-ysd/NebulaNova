<template>
  <div class="container">
    <h1>Welcome to My Nuxt + TypeScript App</h1>
    <p>This is a simple Nuxt 3 application using TypeScript.</p>
    <MyButton label="Click Me" @click="handleClick" />
  </div>
</template>

<script setup lang="ts">
import MyButton from '~/components/MyButton.vue'

const handleClick = (): void => {
  console.log('MyButton clicked!')
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
