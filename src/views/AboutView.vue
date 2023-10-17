<script setup lang="ts">
import { useRoute } from 'vue-router'

const { path, params, query } = useRoute()

const seeRote = () => {
  console.log(path, params, query, '===----')
}
</script>

<template>
  <div class="about">
    <h1 @click="seeRote">This is an about page</h1>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
