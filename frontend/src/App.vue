<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import CraftList from './components/CraftList.vue'
</script>

<template>
  <div id="nav">
    <router-link to="/">Home</router-link>
    <router-link to="/about">About</router-link>
  </div>
  <h1>Welcome to the Kayak Store</h1>
  <router-view />
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

* {
  box-sizing: border-box;
}
</style>
