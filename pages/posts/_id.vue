<template>
  <div class="post">
    <h1>Post ID: {{ id }}</h1>
    <p>This is a dynamic route page.</p>
  </div>
</template>

<script setup lang="ts">
const route = useRoute()
const id: string = route.params.id as string
</script>
  
<style scoped>
.post {
  text-align: center;
  padding: 2rem;
}
</style>
  