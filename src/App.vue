<script setup>
import { RouterLink, RouterView } from 'vue-router'
import AppHeader from './components/AppHeader.vue'
import AppFooter from './components/AppFooter.vue'
</script>

<template>
  <div :class="$style.wrapper">
    <app-header />
    <router-view />
    <app-footer />
  </div>
</template>

<style lang="scss" module>
@import '@/assets/scss/_variables.scss';

html {
  overflow-x: hidden;
  margin-right: calc(-1 * (100vw - 100%));
  // overflow-y: hidden;
  height: 100%;
  scroll-behavior: smooth;
}

::-webkit-scrollbar {
  width: 0px;
  background: transparent;
}

body {
  height: 100%;
  margin: 0;
}

body * {
  text-decoration: none;
  font-size: 16px;
  font-weight: 500;
  color: $text-black;
  font-family:
    -apple-system,
    BlinkMacSystemFont,
    Segoe UI,
    Roboto,
    Oxygen,
    Ubuntu,
    Cantarell,
    Fira Sans,
    Droid Sans,
    Helvetica Neue,
    sans-serif;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-size: 40px;
  line-height: 150%;
  margin: 0;
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

.wrapper {
  min-height: 100%;
  display: flex;
  flex-direction: column;
}
</style>
