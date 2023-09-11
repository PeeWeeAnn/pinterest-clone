<template>
  <footer :class="$style.footer">
    <div :class="$style.wrapper">
      <a :class="$style.footerLink" href="" target="_blank"> Условия предоставления услуг </a>
      <a :class="$style.footerLink" href="" target="_blank"> Политика конфиденциальности </a>
      <a :class="$style.footerLink" href="" target="_blank"> Справка </a>
      <a :class="$style.footerLink" href="" target="_blank"> Приложение для iPhone </a>
      <a :class="$style.footerLink" href="" target="_blank"> Приложение для Android </a>
      <a :class="$style.footerLink" href="" target="_blank"> Пользователи </a>
      <a :class="$style.footerLink" href="" target="_blank"> Коллекции </a>
      <a :class="$style.footerLink" href="" target="_blank"> Покупки </a>
      <a :class="$style.footerLink" href="" target="_blank"> Сегодня </a>
      <a :class="$style.footerLink" href="" target="_blank"> Просмотреть </a>
    </div>
  </footer>
</template>

<script setup></script>

<style lang="scss" module>
@import '@/assets/scss/_variables.scss';

.footer {
  height: 5vh;
  background: $background-white;

  &Link {
    margin-right: 8px;
    font-size: 12px;
  }

  &Link:hover {
    text-decoration: underline;
  }
}

.wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 5vh;
}
</style>
