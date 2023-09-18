<script setup>
import { ref } from 'vue'

import HomeTop from '../components/home/pages/Top.vue'
import HomeSearch from '../components/home/pages/Search.vue'
import HomeSave from '../components/home/pages/Save.vue'
import HomeShop from '../components/home/pages/Shop.vue'
import HomeBottom from '../components/home/pages/Bottom.vue'

let initialAnchor = 'search'
window.location.href = 'http://localhost:5173/#search'

/* const handleScroll = (e) => {
  sectorScroll(e)
}

const sectorScroll = (e) => {
  e.preventDefault()

  const vectorY = e.deltaY

  if (vectorY > 0) {
    switch (initialAnchor) {
      case 'search':
        window.location.href = 'http://localhost:5173/#save'
        initialAnchor = 'save'
        break
      case 'save':
        window.location.href = 'http://localhost:5173/#shop'
        initialAnchor = 'shop'
        break
      case 'shop':
        break
    }
  } else {
    switch (initialAnchor) {
      case 'shop':
        window.location.href = 'http://localhost:5173/#save'
        initialAnchor = 'save'
        break
      case 'save':
        window.location.href = 'http://localhost:5173/#search'
        initialAnchor = 'search'
        break
      case 'search':
        break
    }
  }
} */
</script>

<template>
  <section :class="$style.home" @wheel="handleScroll">
    <home-top id="top" />
    <home-search id="search" />
    <home-save id="save" />
    <home-shop id="shop" />
    <home-bottom id="bottom" />
  </section>
</template>

<style lang="scss" module>
.home {
  flex: 1 1 auto;
}
</style>
