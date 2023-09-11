<template>
  <header :class="$style.header">
    <div :class="$style.wrapper">
      <div :class="$style.logo">
        <a :class="$style.logoLink" href="#">
          <svg-logo :class="$style.logoImage" />
          <h1 :class="$style.logoText">Pinterest</h1>
        </a>
      </div>
      <nav :class="$style.wrapperNavigation">
        <div :class="$style.navigation">
          <a :class="$style.navigationLink" href="">Описание</a>
          <a :class="$style.navigationLink" href="">Бизнес</a>
          <a :class="$style.navigationLink" href="">Блог</a>
        </div>
        <div :class="$style.button">
          <button :class="$style.buttonLogin">Войти</button>
        </div>
        <div :class="$style.button">
          <button :class="$style.buttonSignup">Регистрация</button>
        </div>
      </nav>
    </div>
  </header>
</template>

<script setup>
import SvgLogo from '@/assets/icons/logo.svg?component'
</script>

<style lang="scss" module>
@import '@/assets/scss/_variables.scss';
.header {
  padding: 16px;
  width: calc(100% - 32px);
}

.wrapper {
  display: flex;
  justify-content: space-between;

  &Navigation {
    display: flex;
  }
}

.logo {
  display: flex;
  align-items: center;

  &Link {
    display: flex;
    gap: 4px;
    padding: 0 12px;
  }

  &Image {
    width: 32px;
    height: 32px;
    color: $red;
    fill: currentColor;
  }

  &Text {
    font-size: 20px;
    color: $red;
    letter-spacing: -1px;
  }
}

.navigation {
  display: flex;
  margin: 0 24px 0 0;

  &Link {
    margin: 16px;
  }

  &Link:hover {
    text-decoration: underline;
  }
}

.button {
  display: flex;
  align-items: center;

  &Login {
    background: $red;
    color: $text-white;
    padding: 8px 12px;
    border-radius: 24px;
    margin: 0 10px 0 0;
  }

  &Login:hover {
    background: $hover-red;
  }

  &Signup {
    background: $light-gray;
    padding: 8px 12px;
    border-radius: 24px;
  }

  &Signup:hover {
    background: $hover-light-gray;
  }
}
</style>
