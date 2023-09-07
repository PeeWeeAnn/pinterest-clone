<script setup>
import { RouterLink, RouterView } from 'vue-router'
import AppHeader from './components/AppHeader.vue'
import AppFooter from './components/AppFooter.vue'
</script>

<template>
  <app-header />
  <router-view />
  <app-footer />
</template>

<style lang="scss">
html {
  overflow-x: hidden;
  margin-right: calc(-1 * (100vw - 100%));
  // overflow-y: hidden;
  height: 100%;
  scroll-behavior: smooth;
}

body {
  height: 100%;
  margin: 0;
}

body * {
  text-decoration: none;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-size: 40px;
  font-weight: 500;
  line-height: 150%;
  margin: 0;
}

a {
  font-size: 14px;
  font-weight: 400;
  text-decoration: none;
}

p {
  font-size: 14px;
  font-weight: 400;
}

button {
  margin: 0;
  padding: 0;
  background: transparent;
  border: none;
  cursor: pointer;
}

input {
  outline: none;
}
</style>
