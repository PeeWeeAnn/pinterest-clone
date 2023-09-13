<script setup>
import { ref } from 'vue'

import HomeTop from '../components/home/pages/Top.vue'
import HomeSearch from '../components/home/pages/Search.vue'
import HomeSave from '../components/home/pages/Save.vue'
import HomeShop from '../components/home/pages/Shop.vue'
import HomeBottom from '../components/home/pages/Bottom.vue'

/* const initialX = ref(1000)

const func = (e) => {
  e.preventDefault()

  const vectorY = e.deltaY

  if (vectorY > 0) {
    console.log('Скроллинг вниз ', initialX.value)

    window.scrollTo({
      top: initialX.value,
      behavior: 'smooth'
    })

    if (initialX.value < 5000 || 0) {
      initialX.value += 1000
    }
  } else {
    console.log('Скроллинг вверх', initialX.value)

    window.scrollTo({
      top: initialX.value,
      behavior: 'smooth'
    })

    if (initialX.value > 0) {
      initialX.value -= 1000
    }
  }
} */

let initialAnchor = 'search'
window.location.href = 'http://localhost:5173/#search'

const func = (e) => {
  e.preventDefault()

  const vectorY = e.deltaY

  if (vectorY > 0) {
    switch (initialAnchor) {
      case 'search':
        window.location.href = 'http://localhost:5173/#shop'
        initialAnchor = 'shop'
        break
      case 'shop':
        break
    }
  } else {
    switch (initialAnchor) {
      case 'shop':
        window.location.href = 'http://localhost:5173/#search'
        initialAnchor = 'search'
        break
      case 'search':
        break
    }
  }
}
</script>

<template>
  <section :class="$style.home" @wheel="func">
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
