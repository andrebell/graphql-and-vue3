<script setup>
import { ref } from 'vue'
import useCount from '../composables/useCount';

defineProps({
  msg: String
})

const counter = useCount();
</script>

<template>
  <h1>{{ msg }}</h1>

  <p>
    Recommended IDE setup:
    <a href="https://code.visualstudio.com/" target="_blank">VSCode</a>
    +
    <a href="https://github.com/johnsoncodehk/volar" target="_blank">Volar</a>
  </p>

  <p>
    <a href="https://vitejs.dev/guide/features.html" target="_blank">
      Vite Documentation
    </a>
    |
    <a href="https://v3.vuejs.org/" target="_blank">Vue 3 Documentation</a>
  </p>

  <button type="button" @click="counter.increment">count is: {{ counter.count }}</button>
  <p>
    {{ counter.doubleCount }}
  </p>

</template>

<style scoped>
a {
  color: #42b983;
}
</style>
