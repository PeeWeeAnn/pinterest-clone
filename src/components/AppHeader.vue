<template>
  <header :class="$style.header">
    <div :class="$style.wrapper">
      <div :class="$style.logo">
        <a :class="$style.logoLink" href="#">
          <svg-logo :class="$style.logoImage" />
          <h1 :class="$style.logoText">Pinterest</h1>
        </a>
      </div>
      <div class=""></div>
    </div>
  </header>
</template>

<script setup>
import SvgLogo from '@/assets/icons/logo.svg?component'
</script>

<style lang="scss" module>
@import '@/assets/scss/_variables.scss';
.header {
  background: $red;
}

.logo {
  &Link {
    color: aqua;
  }
  &Image {
    width: 32px;
    height: 32px;
    color: $red;
    fill: currentColor;
  }
  &Text {
  }
}
</style>
